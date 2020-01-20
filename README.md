[Click this link ;-) ](https://github.com/doctor-uz/hbs/blob/master/user.hbs)

# Express handlebars view engine settings in app.js file.

---

// app.js

```javascript
const hbs = require("express-hbs");

app.use("/public", express.static("public"));
app.engine(
    "hbs",
    hbs.express4({
        partialsDir: __dirname + "/views/partials"
    })
);
app.set("view engine", "hbs");
app.set("views", __dirname + "/views/partials");
```

---
