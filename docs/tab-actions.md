---
id: tab-actions
title: TabActions reference
sidebar_label: TabActions
---

`TabActions` is an object containing methods for generating actions specific to tab-based navigators. Its methods expand upon the actions available in [NavigationActions](navigation-actions.html).

The following actions are supported:

### jumpTo

The `jumpTo` action can be used to jump to an existing route in the tab navigator.

- `name` - _string_ - Name of the route to jump to.
- `params` - _object_ - Screen params to merge into the destination route (found in the pushed screen through `route.params`).

```js
import { TabActions } from '@react-navigation/routers';

const jumpToAction = TabActions.jumpTo('Profile', { name: 'Satya' });

navigation.dispatch(jumpToAction);
```
