# innerText VS innerHTML VS textContent

Code example in `index.html`

```js
const navElement = document.querySelector('nav');
console.log({
  innerHTML: navElement.innerHTML,
  textContent: navElement.textContent,
  innerText: navElement.innerText,
});
```

```log
{
  "innerHTML": "\n  <a>Home</a>\n  <a>About</a>\n  <a style=\"display: none\">Contact</a>\n  <a style=\"visibility: hidden\">Pricing</a> <a style=\"opacity: 0\">Login</a>\n",

  "textContent": "\n  Home\n  About\n  Contact\n  Pricing Login\n"

  "innerText": "Home About  Login",

}
```

- [innerHTML](https://developer.mozilla.org/en-US/docs/Web/API/Element/innerHTML): Getting the property returns a string containing the HTML serialization of the element's descendants. or in short that is the string of HTML tags of the node.

- [textContent](https://www.w3schools.com/jsref/prop_node_textcontent.asp): The textContent property sets or returns the text content of the specified node, and all its descendants. All text (ignores CSS).

- [innerText](https://developer.mozilla.org/en-US/docs/Web/API/HTMLElement/innerText):A string representing the rendered text content of an element. Using when getting text as user sees it.
