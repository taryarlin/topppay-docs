## Select2 Component

### Description
<img width="auto" height="100" alt="Screenshot 2022-12-17 at 4 10 50 PM" src="https://myoctocat.com/assets/images/base-octocat.svg">

> Select2 dropdown UI component


### Basic Usage
```html
<select-2 label="From Currency" name="currency_id" placeholder="Choose Currency">
    <option value="1">Kyat</option>
    <option value="2">USD</option>
</select-2>
```
### Expected UI
<img width="1107" alt="Screenshot 2022-12-17 at 4 39 01 PM" src="https://user-images.githubusercontent.com/35889976/208236747-f28dda1a-d374-44b8-a57f-2ceef13cfead.png">

### Available Props

| Prop Name   | Type    | Required | Description                            |
|-------------|---------|----------|----------------------------------------|
| label       | String  | required | For field label                        |
| name        | String  | required | For input name                         |
| placeholder | String  | optional | To display placeholder in select field |
| multiple    | Boolean | optional | For multiple select dropdown           |
| allow-clear | Boolean | optional | To clear selected values               |
| ajax-url    | String  | optional | To show select option with ajax        |
| ajax-method | String  | optional | For ajax request method                |
| id          | String  | optional | To add new id attribute's values       |
| class-name  | String  | optional | To add new class attribute's values    |
| value       | String  | optional | To show selected value                 |
| disabled    | Boolean | optional | To disable the select dropdown         |
| group       | Boolean | optional | For nested values                      |


### Example Expression

```html
<select-2
    value="1"
    label="Exchange Currency"
    required="true"
    placeholder="Choose Currency"
    ajax-url="/data/currencies"
    ajax-method="POST"
>
    <option value="1" selected>
        {{ exchangeRate.currency.name }} ({{ exchangeRate.currency.abbreviation }})
    </option>
</select-2>
```
