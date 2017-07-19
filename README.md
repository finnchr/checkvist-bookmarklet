# Checkvist bookmarklet

## Install

Create new bookmark and paste the following javascript code in location.


```javascript
javascript:(function(){var sel=window.getSelection?window.getSelection():document.getSelection?document.getSelection():document.selection?document.selection.createRange().text:"",a=window,b=document,c=encodeURIComponent,d=new Date().getTime(),e=a.open("https://checkvist.com/checklists/?add_popup=1&d="+d+"&import_cotent=[link:"+c(b.title)+"|"+c(b.location)+"]&import_cotent_note="+c(sel),"bkmk_popup","left="+((a.screenX||a.screenLeft)+10)+",top="+((a.screenY||a.screenTop)+10)+",height=380px,width=480px,resizable=1,alwaysRaised=1");a.setTimeout(function(){e.focus()},300)})();
```
