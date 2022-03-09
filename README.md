## To use React Router

- Include it using 
```
npm install react-router-dom
```

- Connect App to Browser's URL in index.js

```
import { BrowserRouter } from "react-router-dom";
```

- Adding Global Navigation using Link
```
import { Link } from "react-router-dom";
```

- Add routes. ie files in src/routes/{link-used}

- Teach React Router how to render our app at different URLs by creating our first "Route Config" inside index.js
```
import { BrowserRouter, Routes, Route } from "react-router-dom";
import { Home } from "./home.js";
import { About } from "./about.js";
import { Contact } from "./contact.js";

  <BrowserRouter>
    <Routes>
      <Route path="/" element={<App />} />
      <Route path="/" element={<Home />} />
      <Route path="about" element={<About />} />
      <Route path="contact" element={<contact />} />
    </Routes>
  </BrowserRouter>,
```