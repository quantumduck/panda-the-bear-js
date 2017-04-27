# Answers:

1. Change the profile picture:
```javascript
image = $('.profile-image');
image.attr('src', 'https://avatars2.githubusercontent.com/u/25931948?v=3&s=460');
```

2. Change the name.
```javascript
$('h1').text("Quantum Duck");
```

3. Change the "Employment" heading.
```javascript
var original = $('#employment > .info-title').html();
var suitcase_icon = original.substring(0,original.indexOf('Employment'));
$('#employment > .info-title').html(suitcase_icon + "Regrets");
```

4. 
```javascript

```
