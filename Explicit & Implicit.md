# Example of Explicit and Implicit

```javascript


   btnExplicit.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View v) {
                Intent explicitIntent = new Intent(MainActivity.this, SecondActivity.class);
                explicitIntent.putExtra("message", "Hello from MainActivity!");
                startActivity(explicitIntent);
            }
        });

        btnImplicit.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View v) {
                Uri webpage = Uri.parse("https://bongoacademy.com/");
                Intent implicitIntent = new Intent(Intent.ACTION_VIEW, webpage);
                startActivity(implicitIntent);
            }
        });

```

## get Data

```javascript

        String messages=getIntent().getStringExtra("message");
        textView.setText(messages);

```
