# Volcanic-Asia-Documentation (STILL IN PROGRESS)
This repository is a documentation for Volcanic Asia's development environment and methodologies

###Override T&C checked by default:
```  document.getElementById('<T&C ID>').checked = false;``` 

In most cases:``` document.getElementById('user_terms_and_conditions').checked = false; ```

##Multilingual Notes
For sites multi languages that required different fonts accoring to the display language 
``` {% if lang_short == "ja" %}
  <style>
     body, h1, h1 p, h2, h2 p, h3, h3 p, h4, h4 p, h5, h5 p, p, span  {
       font-family:"ヒラギノ角ゴ Pro W3", "Hiragino Kaku Gothic Pro",Osaka, "メイリオ", Meiryo, "ＭＳ Ｐゴシック", "MS PGothic",sans-serif;!important
     }
  </style>
{% endif %} ```
