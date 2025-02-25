# Jetpack Compose Документация

Добро пожаловать в документацию по Jetpack Compose! Здесь вы найдете практические примеры и лучшие практики.

## Быстрый старт

```kotlin title="MainActivity.kt" linenums="1" hl_lines="2-5"
package com.example.myapplication

import android.os.Bundle
import androidx.activity.ComponentActivity
import androidx.activity.compose.setContent
import androidx.activity.enableEdgeToEdge
import androidx.compose.foundation.layout.fillMaxSize
import androidx.compose.foundation.layout.padding
import androidx.compose.material3.Scaffold
import androidx.compose.material3.Text
import androidx.compose.runtime.Composable
import androidx.compose.ui.Modifier
import androidx.compose.ui.tooling.preview.Preview
import com.example.esjiofawdfmyapplication.ui.theme.MyApplicationTheme

class MainActivity : ComponentActivity() {
    override fun onCreate(savedInstanceState: Bundle?) {
        super.onCreate(savedInstanceState)
        enableEdgeToEdge()
        setContent {
            EsjiofawdfMyApplicationTheme {
                Scaffold(modifier = Modifier.fillMaxSize()) { innerPadding ->
                    Greeting(
                        name = "Android",
                        modifier = Modifier.padding(innerPadding)
                    )
                }
            }
        }
    }
}

@Composable
fun Greeting(name: String, modifier: Modifier = Modifier) {
    Text(
        text = "Hello $name!",
        modifier = modifier
    )
}

@Preview(showBackground = true)
@Composable
fun GreetingPreview() {
    EsjiofawdfMyApplicationTheme {
        Greeting("Android")
    }
}
```

### Generic Content

=== "Plain Text"

    tdjskldjs

=== "Unordered List"

    * fdsdkd
    * fjskdldf
    * fsjklfsf

=== "Ordered list"

    1. jskldjfls
    2. jdskljdlsd
    3. dslka

!!! note "Title osdad"

    Lorem jlsakjdlkasjdlkasjl asdlhsal;dh ashdkashdahsdashdashdash ajkdhsjkadhjkashdjh

??? info "djsakldjklasd"

    Lorem jlsakjdlkasjdlkasjl asdlhsal;dh ashdkashdahsdashdashdash ajkdhsjkadhjkashdjh
