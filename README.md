# Read More option
[![Android Arsenal]( https://img.shields.io/badge/Android%20Arsenal-VectorChildFinder-green.svg?style=flat )]( https://android-arsenal.com/details/1/6733 )
[![](https://jitpack.io/v/devsideal/VectorChildFinder.svg)](https://jitpack.io/#devsideal/VectorChildFinder/1.0.0)
[![GitHub license](https://img.shields.io/github/license/dcendents/android-maven-gradle-plugin.svg)](http://www.apache.org/licenses/LICENSE-2.0.html)

Convert your TextView in ExpandableTextView with added options ReadMore/ReadLess.
## Demo
![ReadMoreOption](/assets/rmo-1.0.0.gif)

## Dependency
- Add the dependencies to your gradle files:

#### Step 1. Add it in your root build.gradle at the end of repositories
```gradle
   allprojects {
       repositories {
    	...
    	maven { url 'https://jitpack.io' }
    	}
    }
```

#### Step 2. Add the dependency
```gradle
    dependencies {
        compile 'com.github.devsideal:VectorChildFinder:1.0.0'
     }

```

## Usage
```java

  ReadMoreOption readMoreOption = new ReadMoreOption.Builder(this).build();

  // OR using options to customize

  ReadMoreOption readMoreOption = new ReadMoreOption.Builder(this)
                .textLength(300)
                .moreLabel("MORE")
                .lessLabel("LESS")
                .moreLabelColor(Color.RED)
                .lessLabelColor(Color.BLUE)
                .labelUnderLine(true)
                .build();

  readMoreOption.addReadMoreTo(tv, getString(R.string.dummy_text));

```

## License
```
Copyright 2018 Deven Singh

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
```