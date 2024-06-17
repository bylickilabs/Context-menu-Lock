| Context-menu-Lock |
|---|

### Disable the right-click lock in your HTML code

- [✅] HTML Ready
- [ ] Current problems
- [ ] Miscellaneous

> [!NOTE]
> Useful information to protect your texts and images!
> [!TIP]
> Make your site and/or your pages even better.
> [!IMPORTANT]
> The code protects you and your pages
> [!WARNING]
> Not 100% secure


```yarn
Disable the right-click lock in your HTML code to protect your text and images on,
for example, your Github.io pages. As it should be!
```

---

```yarn
Insert the script after your head for more security.
```

| EXAMPLE |
|---|
```yarn
<head>
  <title>YOUR_SITE_TITLE</title>
...
...
...
</head>
```
---

| SCRIPT |
|---|

```yarn
<!-- LOCK BEGIN -->
<script language="JavaScript1.2">
function disableselect(e){
return false
}
function reEnable(){
return true
}
document.onselectstart=new Function ("return false")
if (window.sidebar){
document.onmousedown=disableselect
document.onclick=reEnable
}
</script>

</head>
<body oncontextmenu="return false">
<script language="JavaScript1.2">
function disableselect(e){
return false
}
function reEnable(){
return true
}
document.onselectstart=new Function ("return false")
if (window.sidebar){
document.onmousedown=disableselect
document.onclick=reEnable
}
</script>
<!-- LOCK END -->
```
---
