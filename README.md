Nithya Ranjana
==============
![Nithya Ranjana Sample Image](https://github.com/EkType/Nithya-Ranjana/raw/385f8d73ea7061dde0598744db0d31b6e6a1a555/Promotion/NithyaRanjana.gif)


Nithya Ranjana is a typeface based on the calligraphic Ranjana script.

Ranjana originated sometime between the 8-11th centuries and is used to write Sanskrit and Nepal Bhasa. It was mainly used for writing Buddhist and Hindu texts in South Asia and is also used for cultural contexts by the Newar people of the Kathmandu valley in Nepal. It has a rich legacy in manuscript calligraphy, stone inscriptions, wood engravings and paintings, but it has had limited digital representation due to its complexity and lack of Unicode support. 

The challenge in creating the Nithya Ranjana font was to strike a balance between Ranjana's heritage and contemporary requirements. Apart from vowels, consonants, numerals and punctuation marks, Nithya Ranjana supports 750+ unique conjuncts used in Nepal Bhasa, Sanskrit and Pali. It includes an additional 500+ character-specific matra forms and matra-specific character forms to correctly and elegantly represent its many unique combinations. It has four stylistic sets, one each for alternate conjuncts and above base matras, and two for 40 Kutakshar forms (monogram-style word marks) making it ideal for historical and contemporary usage.

The Ranjana script does not have Unicode support to date. Hence, this typeface is currently available in 2 versions – Nithya Ranjana DU (based on Devanagari Unicode) and Nithya Ranjana NU (based on Newa Unicode). We hope to update it to Ranjana Unicode as and when the proposal for Ranjana Unicode is accepted.

This project was initiated and sponsored by Murali K. Prahalad, Ph.D. His interest in helping create a modern font for Ranjana is deeply linked to his passion for preserving the world’s Sanskrit heritage for future generations by ensuring the successful transition of Sanskrit into the digital world. He has a keen interest in scripts that facilitated the spread of Sanskrit literature and knowledge across Asia. This font is named after his eldest daughter Nithya, for whose generation he hopes to preserve this tradition.

Nithya Ranjana is designed, engineered and maintained by Ek Type, India with support from Callijatra, Nepal. Key contributors of this project are Tathagata Biswas (Type Design), Noopur Datye (Type Design), Ananda K. Maharjan (Script Expert) and Sarang Kulkarni (Project Management).



License
-------
Nithya Ranjana is licensed under the SIL Open Font License v1.1 (<http://scripts.sil.org/OFL>). To view the copyright and specific terms and conditions, please refer to [OFL.txt](OFL.txt)

### Downloading the font files (TTF files)

The font files can be downloaded from the [releases page.](https://github.com/EkType/Nithya-Ranjana/releases)

### Building the font from source
The Glyphsapp and UFO sources are provided. 
> You can build the fonts using `fontmake` and `gftools` 

### Usage

**Step 1:** Declare Nithya Ranjana as font face in CSS desired file.

```css
@font-face {
  font-family: 'NithyaRanjana';
  src:  url('https://cdn.staticdelivr.com/gh/callijatra/nithya-ranjana-webfont1/main/fonts/NithyaRanjanaDU-Regular.otf') format('otf'),
        url('https://cdn.staticdelivr.com/gh/callijatra/nithya-ranjana-webfont1/main/fonts/NithyaRanjanaDU-Regular.woff2') format('woff2'),
        url('https://cdn.staticdelivr.com/gh/callijatra/nithya-ranjana-webfont1/main/fonts/NithyaRanjanaDU-Regular.woff') format('woff'); /* Fallback format */
  font-weight: 100;
  font-display: swap; 
}

@layer utilities {
  .font-nithya-ranjana {
    font-family: 'NithyaRanjana', sans-serif;
  }

    /* Stylistic Set 1 */
    .font-nithya-ranjana-ss01 {
      font-family: 'NithyaRanjana', sans-serif;
      font-feature-settings: "ss01" 1;
    }
}
```

**Step 2:** Add a class name "font-nithya-ranjana" wherever required. Note that this is Devanagari based Ranjana unicode font. So, the source text needs to be in Devanagari unicode form.

```html
<h1 class="font-nithya-ranjana text-large">ॐ वागिश्वरि मूं</h1>
<h1 class="font-nithya-ranjana-ss01 text-medium">ॐ वागिश्वरि मूं</h1>
```
Nithya Ranjana consists of different stylistic sets and alternate forms. Further style sets can be accessed by setting `font-feature-settings` to `ss01`, `ss02` and so on.


### Getting Involved

Would you like to contribute to the development of this font family? Here is how you can help:

1. Tell us about any bugs you find, or enhancements you would like to see. Send us bug reports, feature enhancements or glyph requests, using the [GitHub Issue Tracker](https://github.com/EkType/Nithya-Ranjana/issues/).

2. Contribute directly to the fonts. This repository contains source files in Glyphsapp and UFO formats. You can make changes as required and build the fonts using `fontmake` and `gftools`. If you wish to contribute directly, please see below how we build the fonts and follow our build process so that we can easily include your contribution, and follow the GitHub pull request process to send your contribution. Write to `info@ektype.in` if you require any assistance in contributing to the family.

