# 0.5.3
- All code TSLinted

# 0.5.2
- Add typings

# 0.5.1
- Fix bug with form failing to initialize without parameters
- Fix bug with form that has validation, failed to initilaize without `validator.attributeNames` parameter;

# 0.5.0
- Changed a way how validatorjs parameters are passed to `reactiveMobXForm` creation function.
- Changed a way how control names are build. from `person.0.firstName` to `person[0].firstname`
- Introduced a `BaseControl` class to keep all logic shared between all types of Controls

# 0.4.0
- Possibility to globally / locally(per form) to set up language of error messages, and how the field name inside error messages is formated.
- Validation of form configuration parameters
- Possibility to set custom error message per rule or rule + field name

# 0.3.3
- Fix Bug, that `Form.reset` did not removed ControlArray children from ui
- Allow `ControlArray` to be the nested child of other `ControlArray`

# 0.3.2 
- `isDirty` property now is computed correctly

# 0.3.1 
- Pass `submitError` property to Form component

# 0.3.0 [Breacking Change]
- Improved logic of working with `fields` array passed into `ControlArray`'s component [Breacking Change].
- No more separate methods for `fields`
- All methods for manipulatin are in `fields.prototype`
- They are: `map, add, insert, remove, swap`

# 0.2.11
- Fix problem with unmountin of `Control*` components. Now unmounting cause correct removing of corresponding `Field` instance from `form.fields`
- Make storing each form in `formStore` as `observableMap`, to correcly react on add/remove form
- Fix bug #2, fields were not mared as untouched on form reset
- Remove dependancy on `React.PropTypes` in favor of `PropTypes`
- Minor updates 