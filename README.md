# target-caching

```html
<target-caching upgrade=a if-wants-to-be=target-caching></target-caching>
<a be-target-caching href=a.html target=myIframeA>A</a>
<a be-target-caching href=b.html target=myIframeB>B</a>
...
<iframe be-grouped=myGroup name=myIframeA></iframe>
<iframe be-grouped=myGroup name=myIframeB></iframe>
```

hyperlink intercepted

1)  Hide all other iframes
2)  Show targetted iframe

need selectable behavior like iron-pages

Take 2

```html
<target-caching upgrade=a if-wants-to-be=target-caching></target-caching>
<a be-target-caching href=a.html target=myIframeA>A</a>
<a be-target-caching href=b.html target=myIframeB>B</a>
...

<channel-ector>
<iframe name=myIframeA></iframe>
<iframe name=myIframeB></iframe>
</channel-ector>
```

1)  Intercept all clicks on hyperlinks
2)  find the target, identify the index within the parent
3)  set the selected index on the parent element.


