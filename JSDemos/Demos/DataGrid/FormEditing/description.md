The DataGrid can use the [Form](/Documentation/ApiReference/UI_Components/dxForm/) component to arrange cell editors when users modify a row. The Form allows users to edit values from [visible and hidden](/Documentation/ApiReference/UI_Components/dxDataGrid/Configuration/columns/#visible) columns (see the `Notes` column).

To use the Form as the row editor UI, specify the following properties:
- **editing**.[mode](/Documentation/ApiReference/UI_Components/dxDataGrid/Configuration/editing/#mode) to *"form"*
- **editing**.[allowUpdating](/Documentation/ApiReference/UI_Components/dxDataGrid/Configuration/editing/#allowUpdating) to **true**

A column's default editor is defined automatically based on this column's [dataType](/Documentation/ApiReference/UI_Components/dxDataGrid/Configuration/columns/#dataType). To customize this editor or replace it with another editor, use the column's [formItem](/Documentation/ApiReference/UI_Components/dxDataGrid/Configuration/columns/#formItem) object. This demo shows how to replace the default editor in the `Notes` column with a [TextArea](/Documentation/ApiReference/UI_Components/dxTextArea/). Refer to the [SimpleItem](/Documentation/ApiReference/UI_Components/dxForm/Item_Types/SimpleItem/) help topic for information on all settings that you can define in the **formItem** object.

You can also set up the edit Form from scratch. The component's [configuration section](/Documentation/ApiReference/UI_Components/dxForm/) lists available settings. Specify these settings in the **editing**.[form](/Documentation/ApiReference/UI_Components/dxDataGrid/Configuration/editing/#form) object. Refer to this object's description for more information about this edit mode's limitations.
