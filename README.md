# react-bootstrap-confirm-modal
Confirm Dialog for react with Bootstrap Modal.


## Example

![Example](https://github.com/gregthebusker/react-confirm-bootstrap/blob/master/img/example.png)

```js
    var Confirm = require('react-confirm-bootstrap');

    var ConfirmAction = React.createClass({
        onConfirm() {
            // Preform your action.
        },

        render() {
            return (
                <Confirm
                    onConfirm={this.onConfirm}
                    body="Are you sure you want to delete this?"
                    confirmText="Confirm Delete"
                    title="Deleting Stuff">
                    <button>Delete Stuff</button>
                </Confirm>
            )
        },
    });
```

### Props
#### body: React.PropTypes.any.isRequired
Body text for the modal.

#### buttonText: React.PropTypes.string
Options text for the initial button.  Is only used if children are not passed.

#### confirmText: React.PropTypes.string
Text for the confirm button in the modal.

#### onConfirm: React.PropTypes.func.isRequired
Function to be called once confirmed.

#### title: React.PropTypes.string.isRequired
Title text for the modal

#### visible: React.PropTypes.bool
Optional initial state if the modal should start open.

#### children: React.PropTypes.any
Node to listen to clicks for.  `react-confirm-bootstrap` render a `react-bootstrap` button by default.
