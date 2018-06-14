## Accordion
An accordion containing collapsible panels.

[![](https://codesandbox.io/static/img/play-codesandbox.svg)](https://codesandbox.io/s/github/grommet/grommet-sandbox?initialpath=accordion&module=%2Fsrc%2FAccordion.js)
## Usage

```javascript
import { Accordion, AccordionPanel } from 'grommet';
<Accordion>
  <AccordionPanel label='Panel 1'>...</AccordionPanel>
  <AccordionPanel label='Panek 2'>...</AccordionPanel>
</Accordion>
```

## Properties

**activeIndex**

Active panel index. If specified, Accordion will be a controlled component. This means that future
panel changes will not work unless you subscribe to onActive function and update activeIndex
accordingly.

```
number
[number]
```

**animate**

Transition content in & out with a slide down animation. Defaults to `true`.

```
boolean
```

**children**

Required. Array of AccordionPanels.

```
[new AccordionPanel(...)]
```

**onActive**

Function that will be called when the active index changes.
It will always send an array with currently active panel indexes.

```
function
```

**multiple**

Allow multiple panels to be opened at once.

```
boolean
```

**messages**

Custom messages for Tabs. Used for accessibility by screen readers. Defaults to `{
  "tabContents": "Tab Contents"
}`.

```
{
  tabContents: string
}
```
  