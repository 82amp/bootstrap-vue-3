# List Group

> List Groups are a flexible and powerful component for displaying a series of content. List Group
> items can be modified to support just about any content within. They can also be used as
> navigation via various props.

<ClientOnly>
  <b-card class="bd-example">
    <b-list-group>
      <b-list-group-item>Cras justo odio</b-list-group-item>
      <b-list-group-item>Dapibus ac facilisis in</b-list-group-item>
      <b-list-group-item>Morbi leo risus</b-list-group-item>
      <b-list-group-item>Porta ac consectetur ac</b-list-group-item>
      <b-list-group-item>Vestibulum at eros</b-list-group-item>
    </b-list-group>
  </b-card>
</ClientOnly>

```html
<b-list-group>
  <b-list-group-item>Cras justo odio</b-list-group-item>
  <b-list-group-item>Dapibus ac facilisis in</b-list-group-item>
  <b-list-group-item>Morbi leo risus</b-list-group-item>
  <b-list-group-item>Porta ac consectetur ac</b-list-group-item>
  <b-list-group-item>Vestibulum at eros</b-list-group-item>
</b-list-group>
```

## Active items

Set the `active` prop on a `<b-list-group-item>` to indicate the current active selection.

<ClientOnly>
  <b-card class="bd-example">
    <b-list-group>
      <b-list-group-item>Cras justo odio</b-list-group-item>
      <b-list-group-item active>Dapibus ac facilisis in</b-list-group-item>
      <b-list-group-item>Morbi leo risus</b-list-group-item>
      <b-list-group-item>Porta ac consectetur ac</b-list-group-item>
      <b-list-group-item>Vestibulum at eros</b-list-group-item>
    </b-list-group>
  </b-card>
</ClientOnly>

```html
<b-list-group>
  <b-list-group-item>Cras justo odio</b-list-group-item>
  <b-list-group-item active>Dapibus ac facilisis in</b-list-group-item>
  <b-list-group-item>Morbi leo risus</b-list-group-item>
  <b-list-group-item>Porta ac consectetur ac</b-list-group-item>
  <b-list-group-item>Vestibulum at eros</b-list-group-item>
</b-list-group>
```

## Disabled items

Set the `disabled` prop on a `<b-list-group-item>` to make it appear disabled (also works with
actionable items. see below).

<ClientOnly>
  <b-card class="bd-example">
    <b-list-group>
      <b-list-group-item disabled>Cras justo odio</b-list-group-item>
      <b-list-group-item>Dapibus ac facilisis in</b-list-group-item>
      <b-list-group-item>Morbi leo risus</b-list-group-item>
      <b-list-group-item disabled>Porta ac consectetur ac</b-list-group-item>
      <b-list-group-item>Vestibulum at eros</b-list-group-item>
    </b-list-group>
  </b-card>
</ClientOnly>

```html
<b-list-group>
  <b-list-group-item disabled>Cras justo odio</b-list-group-item>
  <b-list-group-item>Dapibus ac facilisis in</b-list-group-item>
  <b-list-group-item>Morbi leo risus</b-list-group-item>
  <b-list-group-item disabled>Porta ac consectetur ac</b-list-group-item>
  <b-list-group-item>Vestibulum at eros</b-list-group-item>
</b-list-group>
```

## Actionable list group items

Turn a `<b-list-group-item>` into an actionable _link_ (`<a href="...">`) by specifying either an
`href` prop or ~~[router-link](/docs/reference/router-links) `to`~~ prop.

<ClientOnly>
  <b-card class="bd-example">
    <b-list-group>
      <b-list-group-item href="#some-link">Awesome link</b-list-group-item>
      <b-list-group-item href="#" active>Link with active state</b-list-group-item>
      <b-list-group-item href="#">Action links are easy</b-list-group-item>
      <b-list-group-item href="#foobar" disabled>Disabled link</b-list-group-item>
    </b-list-group>
  </b-card>
</ClientOnly>

```html
<b-list-group>
  <b-list-group-item href="#some-link">Awesome link</b-list-group-item>
  <b-list-group-item href="#" active>Link with active state</b-list-group-item>
  <b-list-group-item href="#">Action links are easy</b-list-group-item>
  <b-list-group-item href="#foobar" disabled>Disabled link</b-list-group-item>
</b-list-group>
```

Or if you prefer `<button>` elements over links, set the `button` prop to `true`.

<ClientOnly>
  <b-card class="bd-example">
    <b-list-group>
      <b-list-group-item button>Button item</b-list-group-item>
      <b-list-group-item button>I am a button</b-list-group-item>
      <b-list-group-item button disabled>Disabled button</b-list-group-item>
      <b-list-group-item button>This is a button too</b-list-group-item>
    </b-list-group>
  </b-card>
</ClientOnly>

```html
<b-list-group>
  <b-list-group-item button>Button item</b-list-group-item>
  <b-list-group-item button>I am a button</b-list-group-item>
  <b-list-group-item button disabled>Disabled button</b-list-group-item>
  <b-list-group-item button>This is a button too</b-list-group-item>
</b-list-group>
```

**Notes:**

- When the prop `button` is `true`, all [link related props](/docs/components/link) (other than
  `active`) and the `tag` prop will have no effect.
- When `href` or ~~`to`~~ are set, the `tag` prop has no effect.

~~Refer to the [Router support](/docs/reference/router-links) reference page for router-link specific
props.~~

## Contextual variants

Use contextual variants to style list items with a stateful background and color, via the `variant`
prop.

<ClientOnly>
  <b-card class="bd-example">
    <b-list-group>
      <b-list-group-item>Default list group item</b-list-group-item>
      <b-list-group-item variant="primary">Primary list group item</b-list-group-item>
      <b-list-group-item variant="secondary">Secondary list group item</b-list-group-item>
      <b-list-group-item variant="success">Success list group item</b-list-group-item>
      <b-list-group-item variant="danger">Danger list group item</b-list-group-item>
      <b-list-group-item variant="warning">Warning list group item</b-list-group-item>
      <b-list-group-item variant="info">Info list group item</b-list-group-item>
      <b-list-group-item variant="light">Light list group item</b-list-group-item>
      <b-list-group-item variant="dark">Dark list group item</b-list-group-item>
    </b-list-group>
  </b-card>
</ClientOnly>

```html
<b-list-group>
  <b-list-group-item>Default list group item</b-list-group-item>
  <b-list-group-item variant="primary">Primary list group item</b-list-group-item>
  <b-list-group-item variant="secondary">Secondary list group item</b-list-group-item>
  <b-list-group-item variant="success">Success list group item</b-list-group-item>
  <b-list-group-item variant="danger">Danger list group item</b-list-group-item>
  <b-list-group-item variant="warning">Warning list group item</b-list-group-item>
  <b-list-group-item variant="info">Info list group item</b-list-group-item>
  <b-list-group-item variant="light">Light list group item</b-list-group-item>
  <b-list-group-item variant="dark">Dark list group item</b-list-group-item>
</b-list-group>
```

Contextual variants also work with action items. Note the addition of the hover styling here not
present in the previous example. Also supported is the `active` state; set it to indicate an active
selection on a contextual list group item.

<ClientOnly>
  <b-card class="bd-example">
    <b-list-group>
      <b-list-group-item href="#">Default list group item</b-list-group-item>
      <b-list-group-item href="#" variant="primary">Primary list group item</b-list-group-item>
      <b-list-group-item href="#" variant="secondary">Secondary list group item</b-list-group-item>
      <b-list-group-item href="#" variant="success">Success list group item</b-list-group-item>
      <b-list-group-item href="#" variant="danger">Danger list group item</b-list-group-item>
      <b-list-group-item href="#" variant="warning">Warning list group item</b-list-group-item>
      <b-list-group-item href="#" variant="info">Info list group item</b-list-group-item>
      <b-list-group-item href="#" variant="light">Light list group item</b-list-group-item>
      <b-list-group-item href="#" variant="dark">Dark list group item</b-list-group-item>
    </b-list-group>
  </b-card>
</ClientOnly>

```html
<b-list-group>
  <b-list-group-item href="#">Default list group item</b-list-group-item>
  <b-list-group-item href="#" variant="primary">Primary list group item</b-list-group-item>
  <b-list-group-item href="#" variant="secondary">Secondary list group item</b-list-group-item>
  <b-list-group-item href="#" variant="success">Success list group item</b-list-group-item>
  <b-list-group-item href="#" variant="danger">Danger list group item</b-list-group-item>
  <b-list-group-item href="#" variant="warning">Warning list group item</b-list-group-item>
  <b-list-group-item href="#" variant="info">Info list group item</b-list-group-item>
  <b-list-group-item href="#" variant="light">Light list group item</b-list-group-item>
  <b-list-group-item href="#" variant="dark">Dark list group item</b-list-group-item>
</b-list-group>
```

### Conveying meaning to assistive technologies

Using color to add meaning only provides a visual indication, which will not be conveyed to users of
assistive technologies – such as screen readers. Ensure that information denoted by the color is
either obvious from the content itself (e.g. the visible text), or is included through alternative
means, such as additional text hidden using the `.visually-hidden` class.

## With badges

Add [badges](/docs/components/badge) to any list group item to show unread counts, activity, and
more with the help of some [flex utility classes](/docs/reference/utility-classes).

<ClientOnly>
  <b-card class="bd-example">
    <b-list-group>
      <b-list-group-item class="d-flex justify-content-between align-items-center">
          Cras justo odio
          <b-badge variant="primary" pill>14</b-badge>
      </b-list-group-item>
      <b-list-group-item class="d-flex justify-content-between align-items-center">
          Dapibus ac facilisis in
          <b-badge variant="primary" pill>2</b-badge>
      </b-list-group-item>
      <b-list-group-item class="d-flex justify-content-between align-items-center">
          Morbi leo risus
          <b-badge variant="primary" pill>1</b-badge>
      </b-list-group-item>
    </b-list-group>
  </b-card>
</ClientOnly>

```html
<b-list-group>
  <b-list-group-item class="d-flex justify-content-between align-items-center">
    Cras justo odio
    <b-badge variant="primary" pill>14</b-badge>
  </b-list-group-item>

  <b-list-group-item class="d-flex justify-content-between align-items-center">
    Dapibus ac facilisis in
    <b-badge variant="primary" pill>2</b-badge>
  </b-list-group-item>

  <b-list-group-item class="d-flex justify-content-between align-items-center">
    Morbi leo risus
    <b-badge variant="primary" pill>1</b-badge>
  </b-list-group-item>
</b-list-group>
```

## Numbered

Add the `numbered` property to opt into numbered list group items. Numbers are generated via CSS (as opposed to a `<ol>s` default browser styling) for better placement inside list group items and to allow for better customization.

<ClientOnly>
  <b-card class="bd-example">
    <b-list-group numbered>
      <b-list-group-item>Cras justo odioo</b-list-group-item>
      <b-list-group-item>Dapibus ac facilisis in</b-list-group-item>
      <b-list-group-item>Morbi leo risus</b-list-group-item>
      <b-list-group-item>Porta ac consectetur ac</b-list-group-item>
      <b-list-group-item>Vestibulum at eros</b-list-group-item>
    </b-list-group>
  </b-card>
</ClientOnly>

```html
<b-card>
  <b-list-group numbered>
    <b-list-group-item>Cras justo odioo</b-list-group-item>
    <b-list-group-item>Dapibus ac facilisis in</b-list-group-item>
    <b-list-group-item>Morbi leo risus</b-list-group-item>
    <b-list-group-item>Porta ac consectetur ac</b-list-group-item>
    <b-list-group-item>Vestibulum at eros</b-list-group-item>
  </b-list-group>
</b-card>
```

These work great with custom content as well.

<ClientOnly>
  <b-card class="bd-example">
    <b-list-group numbered>
      <b-list-group-item class="d-flex justify-content-between align-items-start">
        <div class="ms-2 me-auto">
          <div class="fw-bold">Subheading</div>
          Cras justo odio
        </div>
        <b-badge variant="primary" pill>14</b-badge>
      </b-list-group-item>
      <b-list-group-item class="d-flex justify-content-between align-items-start">
        <div class="ms-2 me-auto">
          <div class="fw-bold">Subheading</div>
          Dapibus ac facilisis in
          </div>
          <b-badge variant="primary" pill>2</b-badge>
      </b-list-group-item>
      <b-list-group-item class="d-flex justify-content-between align-items-start">
        <div class="ms-2 me-auto">
          <div class="fw-bold">Subheading</div>
          Morbi leo risus
        </div>
        <b-badge variant="primary" pill>1</b-badge>
      </b-list-group-item>
    </b-list-group>
  </b-card>
</ClientOnly>

```html
<b-card>
  <b-list-group numbered>
    <b-list-group-item class="d-flex justify-content-between align-items-start">
      <div class="ms-2 me-auto">
        <div class="fw-bold">Subheading</div>
        Cras justo odio
      </div>
      <b-badge variant="primary" pill>14</b-badge>
    </b-list-group-item>
    <b-list-group-item class="d-flex justify-content-between align-items-start">
      <div class="ms-2 me-auto">
        <div class="fw-bold">Subheading</div>
        Dapibus ac facilisis in
      </div>
      <b-badge variant="primary" pill>2</b-badge>
    </b-list-group-item>
    <b-list-group-item class="d-flex justify-content-between align-items-start">
      <div class="ms-2 me-auto">
        <div class="fw-bold">Subheading</div>
        Morbi leo risus
      </div>
      <b-badge variant="primary" pill>1</b-badge>
    </b-list-group-item>
  </b-list-group>
</b-card>
```

**Note:** When using the numbered property, it supercedes the tag property on `b-list-group` and `b-list-group-item`.
With numbered set, the `b-list-group`is always rendered as a `ol`, while the `b-list-group-item` is rendered as a `li`.

## List Groups inside cards

Incorporate list groups into [cards](/docs/components/card). Use the `<b-list-group>` prop `flush`
prop when using cards with `no-body` to make the sides of the list group flush with the card.

<ClientOnly>
  <b-card-group deck>
    <b-card header="Card with list group">
      <b-list-group>
        <b-list-group-item href="#">Cras justo odio</b-list-group-item>
        <b-list-group-item href="#">Dapibus ac facilisis in</b-list-group-item>
        <b-list-group-item href="#">Vestibulum at eros</b-list-group-item>
      </b-list-group>
      <p class="card-text mt-2">
        Quis magna Lorem anim amet ipsum do mollit sit cillum voluptate ex nulla tempor. Laborum
        consequat non elit enim exercitation cillum aliqua consequat id aliqua. Esse ex consectetur
        mollit voluptate est in duis laboris ad sit ipsum anim Lorem.
      </p>
    </b-card>
    <b-card no-body header="Card with flush list group">
      <b-list-group flush>
        <b-list-group-item href="#">Cras justo odio</b-list-group-item>
        <b-list-group-item href="#">Dapibus ac facilisis in</b-list-group-item>
        <b-list-group-item href="#">Vestibulum at eros</b-list-group-item>
      </b-list-group>
      <b-card-body>
        Quis magna Lorem anim amet ipsum do mollit sit cillum voluptate ex nulla tempor. Laborum
        consequat non elit enim exercitation cillum aliqua consequat id aliqua. Esse ex consectetur
        mollit voluptate est in duis laboris ad sit ipsum anim Lorem.
      </b-card-body>
    </b-card>
  </b-card-group>
</ClientOnly>

```html
<b-card-group deck>
  <b-card header="Card with list group">
    <b-list-group>
      <b-list-group-item href="#">Cras justo odio</b-list-group-item>
      <b-list-group-item href="#">Dapibus ac facilisis in</b-list-group-item>
      <b-list-group-item href="#">Vestibulum at eros</b-list-group-item>
    </b-list-group>

    <p class="card-text mt-2">
      Quis magna Lorem anim amet ipsum do mollit sit cillum voluptate ex nulla tempor. Laborum
      consequat non elit enim exercitation cillum aliqua consequat id aliqua. Esse ex consectetur
      mollit voluptate est in duis laboris ad sit ipsum anim Lorem.
    </p>
  </b-card>

  <b-card no-body header="Card with flush list group">
    <b-list-group flush>
      <b-list-group-item href="#">Cras justo odio</b-list-group-item>
      <b-list-group-item href="#">Dapibus ac facilisis in</b-list-group-item>
      <b-list-group-item href="#">Vestibulum at eros</b-list-group-item>
    </b-list-group>

    <b-card-body>
      Quis magna Lorem anim amet ipsum do mollit sit cillum voluptate ex nulla tempor. Laborum
      consequat non elit enim exercitation cillum aliqua consequat id aliqua. Esse ex consectetur
      mollit voluptate est in duis laboris ad sit ipsum anim Lorem.
    </b-card-body>
  </b-card>
</b-card-group>
```

## Horizontal list groups

Set the prop `horizontal` to `true` to change the layout of list group items from vertical to
horizontal across all breakpoints. Alternatively, set `horizontal` to a responsive breakpoint (`sm`,
`md`, `lg` or `xl`) to make a list group horizontal starting at that breakpoint's min-width.
Currently horizontal list groups cannot be combined with `flush` list groups.

**ProTip:** Want equal-width list group items when horizontal? Add the class `flex-fill` to each
list group item.

**Always horizontal:**

<ClientOnly>
  <b-card>
    <b-list-group horizontal>
      <b-list-group-item>Cras justo odio</b-list-group-item>
      <b-list-group-item>Dapibus ac facilisis in</b-list-group-item>
      <b-list-group-item>Morbi leo risus</b-list-group-item>
    </b-list-group>
  </b-card>
</ClientOnly>

```html
<b-card>
  <b-list-group horizontal>
    <b-list-group-item>Cras justo odio</b-list-group-item>
    <b-list-group-item>Dapibus ac facilisis in</b-list-group-item>
    <b-list-group-item>Morbi leo risus</b-list-group-item>
  </b-list-group>
</b-card>
```

**Horizontal at breakpoint `md` and above:**

<ClientOnly>
  <b-card>
    <b-list-group horizontal="md">
      <b-list-group-item>Cras justo odio</b-list-group-item>
      <b-list-group-item>Dapibus ac facilisis in</b-list-group-item>
      <b-list-group-item>Morbi leo risus</b-list-group-item>
    </b-list-group>
  </b-card>
</ClientOnly>

```html
<div>
  <b-list-group horizontal="md">
    <b-list-group-item>Cras justo odio</b-list-group-item>
    <b-list-group-item>Dapibus ac facilisis in</b-list-group-item>
    <b-list-group-item>Morbi leo risus</b-list-group-item>
  </b-list-group>
</div>
```

## Custom content

Add nearly any HTML or component within, even for linked list groups like the one below, with the
help of [flexbox utility classes](/docs/reference/utility-classes).

<ClientOnly>
  <b-card class="bd-example">
    <b-list-group>
      <b-list-group-item href="#" active class="flex-column align-items-start">
         <div class="d-flex w-100 justify-content-between">
            <h5 class="mb-1">List Group item heading</h5>
            <small>3 days ago</small>
         </div>
         <p class="mb-1">
           Donec id elit non mi porta gravida at eget metus. Maecenas sed diam eget risus varius blandit.
         </p>
         <small>Donec id elit non mi porta.</small>
      </b-list-group-item>
      <b-list-group-item href="#" class="flex-column align-items-start">
        <div class="d-flex w-100 justify-content-between">
          <h5 class="mb-1">List Group item heading</h5>
          <small class="text-muted">3 days ago</small>
        </div>
        <p class="mb-1">
        Donec id elit non mi porta gravida at eget metus. Maecenas sed diam eget risus varius blandit.
        </p>
        <small class="text-muted">Donec id elit non mi porta.</small>
      </b-list-group-item>
      <b-list-group-item href="#" disabled class="flex-column align-items-start">
        <div class="d-flex w-100 justify-content-between">
          <h5 class="mb-1">Disabled List Group item</h5>
          <small class="text-muted">3 days ago</small>
        </div>
        <p class="mb-1">
        Donec id elit non mi porta gravida at eget metus. Maecenas sed diam eget risus varius blandit.
        </p>
        <small class="text-muted">Donec id elit non mi porta.</small>
      </b-list-group-item>
    </b-list-group>  
  </b-card>
</ClientOnly>

```html
<b-list-group>
  <b-list-group-item href="#" active class="flex-column align-items-start">
    <div class="d-flex w-100 justify-content-between">
      <h5 class="mb-1">List Group item heading</h5>
      <small>3 days ago</small>
    </div>

    <p class="mb-1">
      Donec id elit non mi porta gravida at eget metus. Maecenas sed diam eget risus varius blandit.
    </p>

    <small>Donec id elit non mi porta.</small>
  </b-list-group-item>

  <b-list-group-item href="#" class="flex-column align-items-start">
    <div class="d-flex w-100 justify-content-between">
      <h5 class="mb-1">List Group item heading</h5>
      <small class="text-muted">3 days ago</small>
    </div>

    <p class="mb-1">
      Donec id elit non mi porta gravida at eget metus. Maecenas sed diam eget risus varius blandit.
    </p>

    <small class="text-muted">Donec id elit non mi porta.</small>
  </b-list-group-item>

  <b-list-group-item href="#" disabled class="flex-column align-items-start">
    <div class="d-flex w-100 justify-content-between">
      <h5 class="mb-1">Disabled List Group item</h5>
      <small class="text-muted">3 days ago</small>
    </div>

    <p class="mb-1">
      Donec id elit non mi porta gravida at eget metus. Maecenas sed diam eget risus varius blandit.
    </p>

    <small class="text-muted">Donec id elit non mi porta.</small>
  </b-list-group-item>
</b-list-group>
```

## Component reference

### `<b-list-group>`

#### Properties

| Property     | Type                  | Default | Description                                                                       |
| ------------ | --------------------- | ------- | --------------------------------------------------------------------------------- |
| `flush`      | `Boolean`             | `false` | When set, renders a flush list group with no left and right borders               |
| `horizontal` | `Boolean` or `String` | `false` | When set, renders the list-group horizontally rather than the default of vertical |
| `numbered`   | `Boolean`             | `false` | When set, renders the list-group as a numbered list                               |
| `tag`        | `String`              | `'div'` | Specify the HTML tag to render instead of the default tag                         |

#### Slots

| Name      | Scoped | Description                                |
| --------- | ------ | ------------------------------------------ |
| `default` | No     | Content (items) to place in the list group |

### `<b-list-group-item>`

#### Properties

| Property   | Type      | Default   | Description                                                                                                         |
| ---------- | --------- | --------- | ------------------------------------------------------------------------------------------------------------------- |
| `action`   | `Boolean` | `false`   | When set, give the item the appearance of having an action. Not needed when props 'to', 'href' or 'button' are used |
| `active`   | `Boolean` | `false`   | When set to `true`, places the component in the active state with active styling                                    |
| `button`   | `Boolean` | `false`   | When true renders the list-group-item as a button element                                                           |
| `disabled` | `Boolean` | `false`   | When set to `true`, disables the component's functionality and places it in a disabled state                        |
| `href`     | `String`  |           | Denotes the target URL of the link for standard a links                                                             |
| `tag`      | `String`  | `'div'`   | Specify the HTML tag to render instead of the default tag                                                           |
| `target`   | `String`  | `'_self'` | Sets the `target` attribute on the rendered link                                                                    |
| `variant`  | `String`  |           | Applies one of the Bootstrap theme color variants to the component                                                  |

#### Slots

| Name      | Scoped | Description                             |
| --------- | ------ | --------------------------------------- |
| `default` | No     | Content to place in the list group item |

<style lang="scss" scoped>
    .bd-example > .card-body > .list-group {
        max-width: 400px;
    }
</style>
