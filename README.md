# Element-F

### Element fullscreen

This userscript allows you to full screen any element on the page with a click! Focus on the main content of an article, fullscreen gifs or videos even if they don't have a fullscreen option, zoom in on pictures, etc...

### Steps

1. Press *shift-ctrl-f* to toggle element selection mode on. The cursor will appear as crosshairs, and the target element will have a slight box-shadow around it
2. Once you've got the element you want selected, just click!

### Customization

You can easily customize the keypress, the style applied to focused elements, and the style applied to the fullscreen element

Edit the lines in the following sections to change those options

#### *Selection Mode Keypress*

```javascript
var toggleElementSelectionKey = "F";
var toggleElementSelectionAlt = false;
var toggleElementSelectionCtrl = true;
```

#### *Target Element Style*

```javascript
var focusedStyle = `box-shadow: 0 3px 6px rgba(0,0,0,0.16),
                                0 3px 6px rgba(0,0,0,0.23),
                                0 3px 6px rgba(255,255,255,0.16),
                                0 3px 6px rgba(255,255,255,0.23) !important;`;
```

#### *Fullscreen Element Style*

```javascript
var fullScreenStyle = "padding: 1em !important;";
```

### Error reporting

I make no promises about prompt replies or maintenance, but if you run into an issue, please follow these steps, and I'll try to look into it:

1. Set `DEBUG` (immediately under the metadata block) to true: `var DEBUG = true;`
2. Launch your browser's javascript console (see [this page](https://lucidchart.zendesk.com/hc/en-us/articles/207323676-How-to-open-the-JavaScript-Console) for help doing so)
3. Repeat the steps that caused the issue
4. Take a screenshot of the console with the Element-F debug messages
5. Send me an email (see @author) with the subject "Element-F Issue" and the screenshots attached

### TODO

- [ ] Update configuration settings to use [GM_config](https://github.com/sizzlemctwizzle/GM_config/)
- [ ] Create Chrome plugin
- [ ] Create Firefox plugin