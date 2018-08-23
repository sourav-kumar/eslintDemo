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
- ESLint works against the configured pluggable rule. |

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
---
### What is [Prettier](https://prettier.io/) ?
<br>
- It is an opinionated code formatter |
- Integrates with many editor |
- Formats code in no time |
- No need of discussion for code format in code review |

---
### Getting Started with Prettier
<br>
- Install the prettier node module
```
    npm install -g prettier
``` 
- Create a configuration file(.prettierrc) |

- Run Prettier on any JS file or Directory that contains JS files |

---

@title[Sample configuration of Prettier]

<p><span class="slide-title">Sample configuration of Prettier</span></p>
<br>

```javascript
module.exports = {
  printWidth: 100,
  semi: true
};
```

---
ESLint and Prettier setup in IDE's [click here](https://confluence.corp.netsuite.com/display/PSGNFP/Code+formatting)



---
## Questions ?

