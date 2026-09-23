package com.jarvis.ai

import android.content.Intent
import android.os.Bundle
import android.provider.Settings
import android.widget.Button
import android.widget.LinearLayout
import android.widget.TextView
import androidx.appcompat.app.AppCompatActivity

class MainActivity : AppCompatActivity() {

    override fun onCreate(savedInstanceState: Bundle?) {
        super.onCreate(savedInstanceState)

        val layout = LinearLayout(this).apply {
            orientation = LinearLayout.VERTICAL
            setPadding(60, 200, 60, 60)
        }

        val title = TextView(this).apply {
            text = "Jarvis AI"
            textSize = 32f
            setPadding(0, 0, 0, 40)
        }

        val status = TextView(this).apply {
            text = "Status: Ready"
            textSize = 16f
            setPadding(0, 0, 0, 40)
        }

        val btnEnable = Button(this).apply {
            text = "Enable Accessibility Service"
            setOnClickListener {
                startActivity(Intent(Settings.ACTION_ACCESSIBILITY_SETTINGS))
            }
        }

        layout.addView(title)
        layout.addView(status)
        layout.addView(btnEnable)

        setContentView(layout)
    }
}