# 4Th Of July Sale

A professional, engaging email template for announcing a sale on the Fourth of July, suitable for retail and e-commerce industries.

![Thumbnail](./thumbnail.png)

## Template Details

- **Industries:** Retail, E-commerce
- **Message Type:** Marketing
- **Tags:** discounts, independenceday, 4thofjulysale

## Files
- `index.html`: The improved, localized, and branded HTML template.
- `template.blade.php`: Ready-to-use Laravel Blade template with `asset()` helpers.
- `assets/`: Directory containing localized images and styles used in the template.

## Usage in Laravel

### 1. Store the Template
Place the `index.html` content in a Blade view (e.g., `resources/views/emails/4th-of-july-sale.blade.php`).

### 2. Handle Assets
Move the content of `assets/` to your public directory (e.g., `public/vendor/mail-templates/4th-of-july-sale/`) and update the paths in the HTML to use the `asset()` helper.

### 3. Send Email
```php
Mail::to($user)->send(new \App\Mail\GenericEmail([
    'view' => 'emails.4th-of-july-sale',
    'data' => [
        // Your dynamic data here
    ]
]));
```

---
*Created with ❤️ by **[LaravelMail.com](https://laravelmail.com)** - Your source for professional email templates.*
