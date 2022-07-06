# React JS Cheat Sheet


### 1. Commands to Install React App 

#### Install Node JS
```
sudo apt-get install nodejs
```

### Install NPM (if not installed)
```
sudo apt-get install npm
```

#### Create React App
```
sudo npm install -g create-react-app
npx create-react-app myfirstreactapp
```

#### Create React Redux App
```
npx create-react-app myfirstreduxapp --template redux
```

#### Create React Redux App with Typescript template
```
npx create-react-app reduxtypescriptapp --template redux-typescript
```

### 2. Commands to install usefull packages

#### Install Bootstrap
Add the css file manually in the index.html 
```
npm i bootstrap react-bootstrap --save
```
#### Install React Routing Dom V6
```
npm i react-router-dom --save
```
import
```
import { 
  BrowserRouter as Router, 
  Routes, 
  Route, 
  Link 
} from "react-router-dom";
```
Uses
```
<Router>
  <Routes>
    <Route path="/" element={ <HomePage /> } />
    <Route path="/about" element={ <AboutPage /> } />
    <Route path="/product/:productId" element={<ProductDetailsPage />} />
    <Route path="/contact" element={ <ContactPage /> }/>
    <Route path="/invoices" element={<Invoices />}>
      <Route path="/:invoiceId" element={<Invoice />} />
      <Route path="/sent" element={<SentInvoices />} />
    </Route>
    <Route path="/*" element={ <PageNotFound /> } />
  </Routes>
</Router>
```

#### Install Redux, Redux Thunk
```
npm i redux react-redux redux-thunk --save
npm i redux-devtools --save-dev
```

### Install Reduxt Toolkit
```
npm i @reduxjs/toolkit
```

#### Install Axios
```
npm i axios --save
```

#### Install Sass / SCSS
```
npm i node-sass --save
```

#### Install Date Picker
```
npm i react-datepicker --save
```

### Install Data Time Picker
```
npm i react-datetime --save
```

### Install Toastify 
```
npm i react-toastify --save
```

### React Select
```
npm i react-select --save
```

### React Flag Select
```
npm i react-flags-select --save
```

### React Currency Select Input Field
```
npm i react-currency-input-field --save
```

### Moment JS 
```
npm i moment --save
```

### Environment 
```
npm i cmd-env --save
```

### Carousel - Swiper [a #] (https://swiperjs.com/react)
```
npm i swiper --save
```

### Install Basic Packages at Once
``` 
npm i bootstrap react-bootstrap node-sass react-toastify redux react-redux redux-thunk axios react-router-dom react-datepicker react-datetime --save
```