# target-caching

```html
<target-caching upgrade=a if-wants-to-be=target-caching></target-caching>
<a be-target-caching href=a.html target=myIframe>A</a>
<a be-target-caching href=b.html target=myIframe>B</a>
...
<iframe name=myIframe></a>
```

hyperlink intercepted

1)  clone of iframe made
2)  If target iframe already has an href, hide it, remove name
3)  give name to clone, never set href directly on clone, hide clone
4)  keep a mapping between href's and iframes somewhere
5)  keep proxy between original iframe and all other iframes?

