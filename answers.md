# Answers:

## Hacking Panda The Bear's Resume

1. Change the profile picture:
```javascript
var images = document.getElementsByClassName('profile-image');
images[0].setAttribute('src', 'https://avatars2.githubusercontent.com/u/25931948?v=3&s=460');
```

2. Change the name.
```javascript
document.getElementsByTagName('h1')[0].innerText = 'Quantum Duck';
```

3. Change the "Employment" heading.
```javascript
var selection = document.querySelector('#employment > .info-title');
var original = selection.innerHTML;
var suitcase_icon =  original.substring(0, original.indexOf('Employment'));
selection.innerHTML = suitcase_icon + 'Regrets'
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

## Adding Elements to the DOM

1. Adding another Pikachu.
```javascript
var pikachu;
for (var i = 0; i < pics.length; i++) {
    if ($(pics[i]).attr('title') === 'Pikachu') {
        pikachu = $(pics[i]).clone();
    }
}
pikachu.appendTo('.portfolio-container');
```

2. Adding 10 more Pikachus.
```javascript
// Using pikachu defined in previous question.
for (i = 0; i < 10; i++) {
    pikachu.clone().appendTo($('.portfolio-container'));
}
```

3. Adding update time:
```javascript
var list = document.getElementsByClassName('bio-info');
var listItem = document.createElement('li');
var leftSpan = document.createElement('span');
var rightSpan = document.createElement('span');
var lastUpdated = document.createTextNode('Page last updated on');
var dateTime = document.createTextNode(Date());
leftSpan.appendChild(lastUpdated);
rightSpan.appendChild(dateTime);
listItem.appendChild(leftSpan);
listItem.appendChild(rightSpan);
listItem.className = 'bio-info-item';
leftSpan.className = 'bio-info-title';
rightSpan.className = 'bio-info-value';
list[0].appendChild(listItem);
```
