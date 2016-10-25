## Font-Password

Font-Password is an ultra lightweight script, created for inputs without type `password`.

### How to use

In your javascript:
```
if('WebkitAppearance' in document.documentElement.style) document.documentElement.className += " webkit";
```

In your css:

```
/* fallback for no webkit browsers */
@font-face {
    font-family: 'pass-mono-400';
    font-style: normal;
    font-weight: 400;
    src: url('pass-mono-400.woff2') format('woff2');
}
input.font-pass {
    -webkit-text-security: disc; 
}
html:not(.webkit) input.font-pass {
    font-family: 'pass-mono-400', monospace;
    font-weight: 400;
} 
```

### Browser support
Font-Password has been tested and works on the following browsers:

* Chrome
* Safari
* Firefox
