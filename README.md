# Volcanic-Asia-Documentation (STILL IN PROGRESS)
This repository is a documentation for Volcanic Asia's development environment and methodologies

###Override T&C checked by default:
```  document.getElementById('<T&C ID>').checked = false;``` 

In most cases:``` document.getElementById('user_terms_and_conditions').checked = false; ```

##Multilingual Notes
#### Custom HTML/liquid for different languages 
to output the language use:  ``` {{ lang_short }} ``` 
##### example for using ``` {{ lang_short }} ``` in conditional

``` 
{% if lang_short == ja %} <!-- 'ja' is language code for japanese --> 
      <section id="japanese_section">
          <!-- japanese HTML blurb -->
      </section>
    {% else %}
        <section id="any_other_language_section">
          <!--  any_other_language HTML blurb -->
      </section>
{% endif %} ``` ```

#####For sites multi languages that required different fonts accoring to the display language 

```
{% if lang_short == "ja" %}
 <style>
     body, h1, h1 p, h2, h2 p, h3, h3 p, h4, h4 p, h5, h5 p, p, span {
       font-family:"ヒラギノ角ゴ Pro W3", "Hiragino Kaku Gothic Pro",Osaka, "メイリオ", Meiryo, "ＭＳ Ｐゴシック", "MS PGothic",sans-serif;!important
     }
  </style>
  {% endif %}
  ```

##Responsive notes
#### Font sizing
first: make sure that all your headings and normal text are using the ```rem``` unit and your ```<html>``` tag contains ```font-size: 62.5% ```

Then inside the media query it better to use ``` html{ font-size: 'value'% } ```
