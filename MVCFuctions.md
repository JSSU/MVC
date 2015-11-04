
#Architecture

##Controllor
+ `/[Controller]/[ActionName]/[Parameters]`

```cs
    public class DefaultController : Controller
    {
        //
        // GET: /Default/
        public string Index()
        {
            return "This is my <b>default</b> action...";
        }
        
        //
        // GET: /Default/Welcome/
        public string Welcome()
        {
            return "This is the Welcome action method...";
        }

    }
```

`http://localhost:xxxx/HelloWorld/Welcome?name=Scott&numtimes=4`
```
public string Welcome(string name, int numTimes = 1) {
     return HttpUtility.HtmlEncode("Hello " + name + ", NumTimes is: " + numTimes);
}
```

+ Controller methods (also known as action methods)

+ .ActionLink(a,b,c)
`Returns an anchor element (a element) for the specified link text, action, controller, route values as a route value dictionary, and HTML attributes as a dictionary.`
  * a-link text
  * b-the name of the controller action


##View
