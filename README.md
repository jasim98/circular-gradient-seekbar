# Circular Gradient Seekbar

Circular Gradient Seekbar is a library which implements custom circular seekbar with ease.

## Installation


#### gradle: 
Add it in your root build.gradle at the end of repositories:
```bash
allprojects {
		repositories {
			...
			maven { url 'https://jitpack.io' }
		}
	}
```

Step 2. Add the dependency
```bash
dependencies {
	implementation 'com.github.jasim98:circular-gradient-seekbar:1.0.0'
	}
```

#### maven:
```bash
<repositories>
		<repository>
		    <id>jitpack.io</id>
		    <url>https://jitpack.io</url>
		</repository>
	</repositories>
```

Step 2. Add the dependency
```bash
<dependency>
	    <groupId>com.github.jasim98</groupId>
	    <artifactId>circular-gradient-seekbar</artifactId>
	    <version>1.0.0</version>
	</dependency>
```


## Usage

```xml
<com.jasim.circulargradientseekbar.CircularSeekBar
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Hello World!"
        app:circle_stroke_width="23dp"
        app:circle_x_radius="100dp"
        app:circle_y_radius="100dp"
        app:end_angle="360"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintRight_toRightOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:max="100"
        app:pointer_color="@android:color/black"
        app:pointer_halo_border_width="5dp"
        app:pointer_halo_width="5dp"
        app:pointer_radius="8dp"
        app:progress="25"
        app:start_angle="180"
        app:circle_gradient_start_color="@android:color/white"
        app:circle_gradient_end_color="@android:color/black"
        app:circle_progress_gradient_start_color="@color/teal_200"
        app:circle_progress_gradient_end_color="@color/purple_200"
        app:circle_progress_gradient_angle="70"
        app:circle_gradient_angle="180"
        />
```
There are several methods that can be used from Kotlin as well,
To setup a listener all you have to do is,

```Kotlin
class CircleSeekBarListener : OnCircularSeekBarChangeListener {
        override fun onProgressChanged(
            circularSeekBar: CircularSeekBar,
            progress: Int,
            fromUser: Boolean
        ) {
            // TODO Insert your code here
        }
    }
```
and create an instance of Circular Gradient Seekbar,

```Kotlin
seekbar.setOnSeekBarChangeListener(CircleSeekBarListener())
```
## Inspired By
Circular SeekBar - devadvance


## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

