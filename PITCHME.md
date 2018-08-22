### ESLint and Prettier


---

### Why do we need Code Linter ?
<br>
- To find the errors in Code|
- To follow same coding standard in team |
- To find the potential errors |
- To auto format the code |

---
### What is [ESLint](https://eslint.org) ?
<br>
- It is a linting tool, written using Node.js. |
- It statically analyzes the code and finds the problematic patterns or code that doesn’t adhere to certain style guidelines. |
- ESLint work against the configured pluggable rule. |

---
### Getting Started with ESLint
<br>
- Install the eslint node module
```
    npm install -g eslint
``` 
- Create a configuration file(.eslintrc) |

- Run ESlint on any JS file or Directory that contains JS files |

---

@title[Sample configuration of ESLint]

<p><span class="slide-title">Sample configuration of ESLint</span></p>
<br>

```javascript
var OFF = 0, WARN = 1, ERROR = 2;

module.exports = exports = {
  "extends": "prettier",
  "plugins": [
        "prettier"
    ],
    "rules": {
        // Possible Errors
        "for-direction": ERROR,
        "block-scoped-var": WARN,
        "no-empty": WARN,
        "no-extra-semi": WARN,
        "no-dupe-args": ERROR,
        
        
        // Best Practices
        "no-unreachable": WARN,
        "no-console": ERROR,
        "vars-on-top": ERROR,
        "no-alert": WARN,
        "eqeqeq": ERROR,

        // Variables
        "no-unused-vars": [ERROR, { "args": "none" }],
    
        // Stylistic - everything here is a warning because of style.
        "array-bracket-spacing": [ WARN, "never" ],
        "no-spaced-func": WARN,
        "no-trailing-spaces": WARN,

        //Prettier Rules
        "prettier/prettier": ["error", {"tabWidth": 4, "singleQuote": true, "printWidth": 100}]
    }

};
```


---?code=sample/go/server.go&lang=golang&title=Golang File

@[1,3-6](Present code found within any repo source file.)
@[8-18](Without ever leaving your slideshow.)
@[19-28](Using GitPitch code-presenting with (optional) annotations.)


```

---?gist=onetapbeyond/494e0fecaf0d6a2aa2acadfb8eb9d6e8&lang=scala&title=Scala GIST

@[23](You can even present code found within any GitHub GIST.)
@[41-53](GIST source code is beautifully rendered on any slide.)
@[57-62](And code-presenting works seamlessly for GIST too, both online and offline.)

---

## Template Help

- [Code Presenting](https://github.com/gitpitch/gitpitch/wiki/Code-Presenting)
  + [Repo Source](https://github.com/gitpitch/gitpitch/wiki/Code-Delimiter-Slides), [Static Blocks](https://github.com/gitpitch/gitpitch/wiki/Code-Slides), [GIST](https://github.com/gitpitch/gitpitch/wiki/GIST-Slides) 
- [Custom CSS Styling](https://github.com/gitpitch/gitpitch/wiki/Slideshow-Custom-CSS)
- [Slideshow Background Image](https://github.com/gitpitch/gitpitch/wiki/Background-Setting)
- [Slide-specific Background Images](https://github.com/gitpitch/gitpitch/wiki/Image-Slides#background)
- [Custom Logo](https://github.com/gitpitch/gitpitch/wiki/Logo-Setting), [TOC](https://github.com/gitpitch/gitpitch/wiki/Table-of-Contents), and [Footnotes](https://github.com/gitpitch/gitpitch/wiki/Footnote-Setting)

---

## Go GitPitch Pro!

<br>
<div class="left">
    <i class="fa fa-user-secret fa-5x" aria-hidden="true"> </i><br>
    <a href="https://gitpitch.com/pro-features" class="pro-link">
    More details here.</a>
</div>
<div class="right">
    <ul>
        <li>Private Repos</li>
        <li>Private URLs</li>
        <li>Password-Protection</li>
        <li>Image Opacity</li>
        <li>SVG Image Support</li>
    </ul>
</div>

---

### Questions?

<br>

@fa[twitter gp-contact](@gitpitch)

@fa[github gp-contact](gitpitch)

@fa[medium gp-contact](@gitpitch)

---?image=assets/image/gitpitch-audience.jpg

@title[Download this Template!]

### Get your presentation started!
### [Download this template @fa[external-link gp-download]](https://gitpitch.com/template/download/netflix)

