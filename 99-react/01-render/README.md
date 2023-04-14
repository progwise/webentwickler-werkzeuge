# Foundation

```
<html>
    <body>
        <script src="https://unpkg.com/react@17/umd/react.development.js" crossorigin></script>
        <script src="https://unpkg.com/react-dom@17/umd/react-dom.development.js" crossorigin></script>

        <div id="root"></div>

        <script>
            let reactElement = React.createElement("h1", null, "Hello, world!");
            ReactDOM.render( reactElement, document.getElementById('root'));
        </script>
    </body>

</html>
```