## Image Upload Component

### Description
<img width="auto" height="100" alt="Screenshot 2022-12-17 at 4 10 50 PM" src="https://myoctocat.com/assets/images/base-octocat.svg">

**Component Name - ImageUpload.vue**
> To easily display image preview and image upload with one component


### Basic Usage
```html
<image-upload label="Slip Photo" name="photo"></image-upload>
```

### Expected UI
<img width="281" alt="Screenshot 2022-12-17 at 4 10 50 PM" src="https://user-images.githubusercontent.com/35889976/208235824-167e677c-2d81-4aa4-9f19-65a5778347f1.png">

### Available Props

| Prop Name       | Type    | Description                           | Required |
|-----------------|---------|---------------------------------------|----------|
| label           | String  | For field label                       | required |
| name            | String  | Form input name                       | required |
| wrapper-classes | String  | To add custom classes to parent div   | optional |
| src             | String  | To show existing image                | optional |
| required        | Boolean | To add red asterisk (*) sign in label | optional |

### Full Expression

```html
<image-upload 
  label="Slip Photo" 
  name="photo"
  wrapper-classes="mb-4 bg-rose-600"
  required="true"
  src="www.toppay.com/public/image/flower.png"
>
</image-upload>
```
