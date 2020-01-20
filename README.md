[Click this link ;-) ](https://github.com/doctor-uz/hbs/blob/master/user.hbs)

# Express handlebars view engine settings in app.js file.

---

// app.js

```javascript
const hbs = require('express-hbs‘);
```

// Serve static resources

```javascript
app.use("/public", express.static("public"));
```

// Render View

```javascript
app.engine('hbs', hbs.express4({
	partialsDir: __dirname + '/views/partials' }));
app.set('view engine', 'hbs‘);
app.set('views', __dirname + '/views/partials');
```

---
