```jsx
const initial = {
  isOpen: false,
  group: {
    id: '1001',
    type: 'group',
    avatar: null,
    name: 'Example group',
    shortname: null,
    about: null,
  },
  context: {
    name: {
      error: null,
      pending: false
    },
    shortname: {
      error: null,
      pending: false
    },
    about: {
      error: null,
      pending: false
    },
    avatar: {
      error: null,
      pending: false
    }
  }
};
initialState = initial;

<div>
  <Button theme="primary" onClick={() => setState({ isOpen: true })}>Edit Group</Button>
  {
    state.isOpen
      ? <EditGroupModal
          group={state.group}
          context={state.context}
          onClose={() => setState(initial)}
          onSubmit={console.debug}
        />
      : null
  }
</div>
```
