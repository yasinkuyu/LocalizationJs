## LocalizationJs
LocalizationJs is (native) Javascript base Localization library. Dynamically can define an unlimited number of languages. 
    
### Install

        bower install localization-js
        
<script type="text/javascript" src="bower_components/localization-js/localization.min.js"></script>
        
###Simple Usage

        // <script type="text/javascript" src="bower_components/localization-js/localization.min.js"></script>
        // Define language elements
        var locales = {
            "tr_TR": {
                "homepage": "Anasayfa",
                "info": "Bilgi",
                "help": "Yardım"
            },
            "en_US": {
                "homepage": "Homepage",
                "info": "Info",
                "help": "Help"
            }
        };
        
        var loc = new Localization();
            loc.setLang("tr_TR"); //default
            loc.set(locales);
            
            console.log(loc.get("homepage"));

###Dynamically
        "tr_TR": {
             "homepage": "Anasayfa",
             "info": "Bilgi",
             "help": "Yardım"
        },
        "en_US": {
             "homepage": "Homepage",
             "info": "Info",
             "help": "Help",
             ....
        },
        "en_GB": {},
        "en_NZ": {},
        "ar_EG: {}
        
        -> loc.setLang("ar_EG");

###Language Codes 
https://msdn.microsoft.com/en-us/library/ms533052(v=vs.85).aspx

###RTL Support (Right to Left)

        "ar_EG": {
            "rtl": true,
             ...
        } 
        
        if(loc.get("rtl"))
        {
           console.log("Right to left language");
        }

##Contribution
Fork & Pull Request

###License
The MIT License

Create multi-language structure with ASP.NET MVC

https://github.com/yasinkuyu/Localization

Created 2015 Yasin Kuyu - @yasinkuyu
