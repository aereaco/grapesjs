<!-- Generated by documentation.js. Update this documentation by updating the source code. -->

## Selector



### Properties

*   `name` **[String][1]** Selector name, eg. `my-class`
*   `label` **[String][1]** Selector label, eg. `My Class`
*   `type` **[Number][2]?** Type of the selector. 1 (class) | 2 (id)
*   `active` **[Boolean][3]?** If not active, it's not selectable by the Style Manager.
*   `private` **[Boolean][3]?** If true, it can't be seen by the Style Manager, but it will be rendered in the canvas and in export code.
*   `protected` **[Boolean][3]?** If true, it can't be removed from the attached component.

### toString

Get selector as a string.

#### Examples

```javascript
// Given such selector: { name: 'my-selector', type: 2 }
console.log(selector.toString());
// -> `#my-selector`
```

Returns **[String][1]**&#x20;

### getName

Get selector name.

#### Examples

```javascript
// Given such selector: { name: 'my-selector', label: 'My selector' }
console.log(selector.getName());
// -> `my-selector`
```

Returns **[String][1]**&#x20;

### getLabel

Get selector label.

#### Examples

```javascript
// Given such selector: { name: 'my-selector', label: 'My selector' }
console.log(selector.getLabel());
// -> `My selector`
```

Returns **[String][1]**&#x20;

### setLabel

Update selector label.

#### Parameters

*   `label` **[String][1]** New label

#### Examples

```javascript
// Given such selector: { name: 'my-selector', label: 'My selector' }
selector.setLabel('New Label')
console.log(selector.getLabel());
// -> `New Label`
```

### getActive

Get selector active state.

Returns **[Boolean][3]**&#x20;

### setActive

Update selector active state.

#### Parameters

*   `value` **[Boolean][3]** New active state

[1]: https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/String

[2]: https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Number

[3]: https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Boolean
