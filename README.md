# AB_web_tools

AB_web_tools (v2.0.0) is a build process for modern web projects.

## Features

- [Open Graph](https://ogp.me/)
- [Twitter Card](https://developer.twitter.com/en/docs/twitter-for-websites/cards/overview/abouts-cards)
- [Facebook Insights](https://www.facebook.com/business/insights/tools/audience-insights)

## Tasks

- [autoprefixer]()
- [browser-sync]()
- [eslint]()
- [imagemin-cli]()
- [onchange]()
- [postcss-cli]()
- [sass]()
- [stylelint]()
- [uglify-js]()

## Scripts

- **npm run serve**
  
  ```browser-sync start --server --files 'build/css/*.css, build/js/*.js, **/*.html, !node_modules/**/*.html'```

- **npm run eslint**

  ```eslint src/js```

- **npm run imagemin**
  
  ```mkdir -p build && mkdir -p build/images && imagemin src/images/* -o build/image```

- **npm run autoprefixer**
  
  ```postcss -u autoprefixer build/css/*.css```

- **npm run scss**
  
  ```mkdir -p build && mkdir -p build/css && sass src/scss/main.scss build/css/main.css```

- **npm run lint-css**
  
  ```stylelint src/scss/*.scss --syntax scss || true```

- **npm run uglify**
  
  ```mkdir -p build && mkdir -p build/js && uglifyjs src/js/*.js -m -o build/js/app.js && uglifyjs src/js/*.js -m -c -o build/js/app.min.js```