# API Reference

## Get3DModelLoader
```kotlin
class Get3DModelLoader(context: Context) {
    fun generate3DModel(inputImage: Bitmap): ByteArray
}
```

## FilamentViewer
```kotlin
class FilamentViewer(context: Context) : GLSurfaceView(context) {
    fun loadModel(modelData: ByteBuffer)
}
```

## ModelViewer (Composable)
```kotlin
@Composable
fun ModelViewer(
    modelData: ByteArray?,
    modifier: Modifier = Modifier
)
```

## Get3DApp (Main Composable)
```kotlin
@Composable 
fun Get3DApp()
```

## Key Parameters
- `inputImage`: Input bitmap (224x224 recommended)
- `modelData`: Output 3D model data