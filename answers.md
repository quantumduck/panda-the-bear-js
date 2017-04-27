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

4. Remove the time travel skill.
```javascript
$('#time-travel').parent().remove();
```

5. Change the background colour of the body.
```javascript
$('body').css('background-color','#123456');
```

6. Change the background colour of the highlight class.
```javascript
$('.highlight').css('background-color', '#654321');
```

7. Change the font family of h1 to monospace.
```javascript
$('h1').css('font-family', 'monospace');
```

8. Change the colour of the round icons in the sidebar.
```javascript
$('.action-icon-bg').css('background-color', '#FEDCBA');
```

9. Change the placeholder in the contact form.
```javascript
$('#name').attr('placeholder', 'Identify Yourself!');
```

10. Ditto.
```javascript
$('#message').attr('placeholder', 'State your business!');
```

11. Change the default value in the form field.
```javascript
$('#name').attr('value', 'Your Nemesis');
```

12. Ditto.
```javascript
$('#email').attr('value', 'koalathebear@gmail.com');
```

13. Change the submit button text.
```javascript
$('#submit').attr('value', 'En Garde!');
```
