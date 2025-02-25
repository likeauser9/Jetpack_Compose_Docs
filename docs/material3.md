# Material Design 3 в Jetpack Compose

## Настройка темы

```kotlin title="bubble_sort.py"
// 1. Добавьте зависимость в build.gradle
dependencies {
    implementation 'androidx.compose.material3:material3:1.2.0'
}

// 2. Создайте тему
@Composable
fun MyAppTheme(
    content: @Composable () -> Unit
) {
    MaterialTheme(
        colorScheme = lightColorScheme(
            primary = Color(0xFF006C4C),
            secondary = Color(0xFF4A6355)
        ),
        typography = Typography(
            bodyLarge = TextStyle(
                fontFamily = FontFamily.Default,
                fontWeight = FontWeight.Normal,
                fontSize = 16.sp
            )
        ),
        content = content
    )
}
```
