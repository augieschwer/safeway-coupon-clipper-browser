# safeway-coupon-clipper-browser
A browser automation tool for clipping Safeway digital coupons

From https://www.reddit.com/r/Frugal/comments/bi5szz/automatic_safeway_coupon_clipper/

Place the following into a bookmarklet:

```javascript:javascript:(function(){function sleep(e){return new Promise(t=>setTimeout(t,e))}async function click(){for(var e=document.getElementsByClassName("btn load-more")[0];void 0!==e;)e.click(),e=document.getElementsByClassName("btn load-more")[0],await sleep(500);var t=document.getElementsByClassName("btn-primary");for(i=0;i<t.length;i++)t[i].click()}click();}());```

click the bookmark after you are logged into Safeway.com
