---
wrapper_template: '_layouts/docs.html'
context:
  title: Switch | Components
---

# Switch

<hr>

You can use this switch component to display on and off content, such as for settings or simple controls. By changing the `aria-checked` attribute from true or false will animate the switch on/off.

<div class="embedded-example"><a href="/docs/examples/patterns/switch/" class="js-example">
View example of the switch pattern
</a></div>

## Accessibility

### How it works

The switch component is used to display on and off content. It includes the `role=”switch”` attribute so the screen reader distinguishes it from a checkbox. The `span` with class name `p-switch__label` acts as the label, and is associated with the status of the switch input.

The element is focusable, and the `Spacebar` changes the state of the switch the same way a click would.

### Considerations

This component strives to follow [WCAG 2.1 (level AA) guidelines](https://www.w3.org/TR/WCAG21/), and care must be taken to ensure this effort is maintained when the component is implemented across other projects. This section offers advice to that effect:

- Each switch should have a clear and concise label
- Adding `aria-checked=”true”` or `aria-checked=”false”` will set the switch to on or off respectively.
- `aria-readonly` is set to false as default, meaning the user can change the value of the switch. Change this to true if the switch is meant to be read only (i.e. disabled).

### Resources

- [WAI-ARIA names and descriptions definition](https://www.w3.org/TR/wai-aria-practices-1.1/#names_and_descriptions_definition)
- [MDN Web accessibility - Switch role](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/switch_role)
- Guidelines:
  - [4.1.2 Name, Role, Value](https://www.w3.org/TR/UNDERSTANDING-WCAG20/ensure-compat-rsv.html)
  - [ 3.2.2 On Input](https://www.w3.org/WAI/WCAG21/Understanding/on-input)

## Import

To import just this component into your project, copy the snippet below and include it in your main Sass file.

```scss
// import Vanilla and include base mixins
// this only needs to happen once in a given project
@import 'vanilla-framework';
@include vf-base;

@include vf-p-switch;
```

For more information see [Customising Vanilla](/docs/customising-vanilla/) in your projects, which includes overrides and importing instructions.
