# Badge

Documentation and examples for badges, our small count and labeling component.

## Examples

Badges scale to match the size of the immediate parent element by using relative font sizing and em units. As of v5, badges no longer have focus or hover styles for links

### Headings

<ClientOnly>
    <b-card class="mt-2">
        <h1>Example heading <b-badge>New</b-badge></h1>
        <h2 class="border-0 pb-0">Example heading <b-badge>New</b-badge></h2>
        <h3>Example heading <b-badge>New</b-badge></h3>
        <h4>Example heading <b-badge>New</b-badge></h4>
        <h5>Example heading <b-badge>New</b-badge></h5>
        <h6>Example heading <b-badge>New</b-badge></h6>
    </b-card>
</ClientOnly>

```html
<h1>Example heading <b-badge>New</b-badge></h1>
<h2>Example heading <b-badge>New</b-badge></h2>
<h3>Example heading <b-badge>New</b-badge></h3>
<h4>Example heading <b-badge>New</b-badge></h4>
<h5>Example heading <b-badge>New</b-badge></h5>
<h6>Example heading <b-badge>New</b-badge></h6>
```

### Buttons

Badges can be used as part of links or buttons to provide a counter.

<ClientOnly>
    <b-card>
        <b-button variant="primary">
            Notifications <b-badge variant="light">4</b-badge>
        </b-button>
    </b-card>
</ClientOnly>

```html
<b-button variant="primary">Notifications <b-badge variant="light">4</b-badge></b-button>
```

Note that depending on how they are used, badges may be confusing for users of screen readers and similar assistive technologies. While the styling of badges provides a visual cue as to their purpose, these users will simply be presented with the content of the badge. Depending on the specific situation, these badges may seem like random additional words or numbers at the end of a sentence, link, or button.

Unless the context is clear (as with the “Notifications” example, where it is understood that the “4” is the number of notifications), consider including additional context with a visually hidden piece of additional text.

### Positioned

Use utilities to modify a `.badge` and position it in the corner of a link or button.

<ClientOnly>
    <b-card>
        <b-button variant="primary" class="position-relative">
            Inbox
            <b-badge variant="danger" text-indicator>
                99+
                <span class="visually-hidden">unread messages</span>
            </b-badge>
        </b-button>
    </b-card>
</ClientOnly>

```html
<b-button variant="primary" class="position-relative">
  Inbox
  <b-badge variant="danger" text-indicator>
    99+
    <span class="visually-hidden">unread messages</span>
  </b-badge>
</b-button>
```

You can also replace the `.badge` class with a few more utilities without a count for a more generic indicator.

<ClientOnly>
    <b-card>
        <b-button variant="primary" class="position-relative">
            Inbox
            <b-badge variant="danger" dot-indicator>
                <span class="visually-hidden">New alerts</span>
            </b-badge>
        </b-button>
    </b-card>
</ClientOnly>

```html
<b-button variant="primary" class="position-relative">
  Inbox
  <b-badge variant="danger" dot-indicator>
    <span class="visually-hidden">New alerts</span>
  </b-badge>
</b-button>
```

## Background colors

Add any of the following variants via the `variant` prop to change the appearance of a `<b-badge>`: `default`, `primary`, `success`, `warning`, `info`, and `danger`. If no variant is specified `default` will be used.

<ClientOnly>
    <b-card>
        <b-badge variant="primary">Primary</b-badge>
        <b-badge variant="secondary">Secondary</b-badge>
        <b-badge variant="success">Success</b-badge>
        <b-badge variant="danger">Danger</b-badge>
        <b-badge variant="warning">Warning</b-badge>
        <b-badge variant="info">Info</b-badge>
        <b-badge variant="light">Light</b-badge>
        <b-badge variant="dark">Dark</b-badge>
    </b-card>
</ClientOnly>

```html
<b-badge variant="primary">Primary</b-badge>
<b-badge variant="secondary">Secondary</b-badge>
<b-badge variant="success">Success</b-badge>
<b-badge variant="danger">Danger</b-badge>
<b-badge variant="warning">Warning</b-badge>
<b-badge variant="info">Info</b-badge>
<b-badge variant="light">Light</b-badge>
<b-badge variant="dark">Dark</b-badge>
```

::: tip Conveying meaning to assistive technologies
Using color to add meaning only provides a visual indication, which will not be conveyed to users of assistive technologies – such as screen readers. Ensure that information denoted by the color is either obvious from the content itself (e.g. the visible text), or is included through alternative means, such as additional text hidden with the `.visually-hidden` class.
:::

## Pill badges

Use the `pill` prop to make badges more rounded with a larger border-radius.

<ClientOnly>
    <b-card>
        <b-badge variant="primary" pill>Primary</b-badge>
        <b-badge variant="secondary" pill>Secondary</b-badge>
        <b-badge variant="success" pill>Success</b-badge>
        <b-badge variant="danger" pill>Danger</b-badge>
        <b-badge variant="warning" pill>Warning</b-badge>
        <b-badge variant="info" pill>Info</b-badge>
        <b-badge variant="light" pill>Light</b-badge>
        <b-badge variant="dark" pill>Dark</b-badge>
    </b-card>
</ClientOnly>

```html
<b-badge variant="primary" pill>Primary</b-badge>
<b-badge variant="secondary" pill>Secondary</b-badge>
<b-badge variant="success" pill>Success</b-badge>
<b-badge variant="danger" pill>Danger</b-badge>
<b-badge variant="warning" pill>Warning</b-badge>
<b-badge variant="info" pill>Info</b-badge>
<b-badge variant="light" pill>Light</b-badge>
<b-badge variant="dark" pill>Dark</b-badge>
```

## Actionable badges

Quickly provide actionable badges with ~~hover~~ and ~~focus~~ states by specifying either the `href` prop (links) or `to` prop (router-links):

<ClientOnly>
  <b-card>
    <b-badge href="#" variant="primary">Primary</b-badge>
    <b-badge href="#" variant="secondary">Secondary</b-badge>
    <b-badge href="#" variant="success">Success</b-badge>
    <b-badge href="#" variant="danger">Danger</b-badge>
    <b-badge href="#" variant="warning">Warning</b-badge>
    <b-badge href="#" variant="info">Info</b-badge>
    <b-badge href="#" variant="light">Light</b-badge>
    <b-badge href="#" variant="dark">Dark</b-badge>
  </b-card>
</ClientOnly>

```html
<b-badge href="#" variant="primary">Primary</b-badge>
<b-badge href="#" variant="secondary">Secondary</b-badge>
<b-badge href="#" variant="success">Success</b-badge>
<b-badge href="#" variant="danger">Danger</b-badge>
<b-badge href="#" variant="warning">Warning</b-badge>
<b-badge href="#" variant="info">Info</b-badge>
<b-badge href="#" variant="light">Light</b-badge>
<b-badge href="#" variant="dark">Dark</b-badge>
```

## Component reference

### Properties

| Property         | Type      | Default       | Description                                                        |
| ---------------- | --------- | ------------- | ------------------------------------------------------------------ |
| `dot-indicator`  | `Boolean` | `false`       |
| `text-indicator` | `Boolean` | `false`       |
| `pill`           | `Boolean` | `false`       | When set to 'true', renders the badge in pill style                |
| `variant`        | `String`  | `'secondary'` | Applies one of the Bootstrap theme color variants to the component |

### Slots

| Name      | Description                   |
| --------- | ----------------------------- |
| `default` | Content to place in the badge |
