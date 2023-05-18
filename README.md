# Flutter Validatorless

This package provides a means to validate text inputs on the flutter and was inspired by Yup

## how to use

   ```
   dependencies:
  # Use the latest version available. Any is just a placeholder
  validatorless: any
   ```

   ```
   TextFormField(
  decoration: InputDecoration(
    labelText: 'User e-mail',
  ),
  validator: Validatorless.multiple([
     Validatorless.email('The field must be an email'),
     Validatorless.required('The field is obligatory')
  ]),
)
   ```

or

   ```
   TextFormField(
  decoration: InputDecoration(
    labelText: 'CPF',
  ),
  validator: Validatorless.cpf('CPF not is valid'),
)
   ```

### Validatorless options 

   ```
   Validatorless.required(String)
  Validatorless.email(String)
  Validatorless.min(int, String)
  Validatorless.max(int, String)
  Validatorless.between(int, int, String)
  Validatorless.number(String)
  Validatorless.cpf(String)
  Validatorless.cnpj(String)
  Validatorless.date(String)
  Validatorless.compare(TextEditingController, String)
  Validatorless.numbersBetweenInterval(Double, Double, String)
  Validatorless.onlyCharacters(String)
  Validatorless.regex(RegExp, String)
   ```
