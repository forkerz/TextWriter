# TextWriter
Animate your text like never before

## Add dependency

Add this in your root build.gradle at the end of repositories:

```bash
allprojects {
	repositories {
		...
		maven { url 'https://jitpack.io' }
	}
}		
```
Add this in your app level gradle:

```bash
implementation 'com.github.sarnavakonar:TextWriter:v1.0'
```

## Initialization

Initialize the TextWriter:

```bash
TextWriter textWriter;

textWriter = findViewById(R.id.tw);
```

## Customization

Customize according to your need:

```bash
textWriter
         .setWidth(12)
         .setDelay(30)
         .setColor(Color.BLUE)
         .setConfig(TextWriter.Configuration.INTERMEDIATE)
         .setSizeFactor(50f)
         .setLetterSpacing(25f)
         .setText("LIVERPOOL FC")
         .setListener(new TextWriter.Listener() {
          	@Override
          	public void WritingFinished() {

			//do stuff after animation is finished
                }
          })
         .startAnimation();
```

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License
[MIT](https://choosealicense.com/licenses/mit/)
