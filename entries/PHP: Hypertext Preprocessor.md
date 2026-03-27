# PHP: Hypertext Preprocessor

# 🐘 PHP: Hypertext Preprocessor

**PHP** (recursive acronym for **PHP: Hypertext Preprocessor**) is a popular general-purpose scripting language especially suited for web development. Created by Danish-Canadian programmer Rasmus Lerdorf in 1994, it now powers over 75% of all websites.

---

## 📜 History

- **1994** – Rasmus Lerdorf creates **Personal Home Page Tools** to track visits to his online resume.
- **1995** – PHP/FI (Form Interpreter) is released, adding database support.
- **1997** – PHP 3 is released; the name becomes the recursive **PHP: Hypertext Preprocessor**.
- **2000** – PHP 4 launches with the Zend Engine.
- **2004** – PHP 5 introduces robust object-oriented programming.
- **2015** – PHP 7 delivers massive performance gains and scalar type declarations.
- **2020** – PHP 8 releases with the JIT (Just-In-Time) compiler.
- **2023** – PHP 8.3 introduces typed class constants and deep-cloning of readonly properties.

---

## ✨ Key Features

- **Server-side execution** – Runs on a web server, generating dynamic HTML.
- **Beginner-friendly** – C-like syntax with extensive documentation and a huge community.
- **Database integration** – Native support for MySQL, PostgreSQL, SQLite, and more via PDO.
- **Cross-platform** – Works on Windows, Linux, macOS, and all major web servers (Apache, Nginx, IIS).
- **High performance** – PHP 8+ offers exceptional speed, especially with the JIT compiler.
- **Type safety** – Modern PHP supports strict typing, union types, and mixed types.

---

## 🧪 Code Example

```php
<?php

declare(strict_types=1);

$greeting = "Hello, World! 🌍";
echo $greeting;

function calculateTotal(float $price, int $quantity, float $taxRate = 0.10): float {
    $subtotal = $price * $quantity;
    return $subtotal + ($subtotal * $taxRate);
}

$total = calculateTotal(24.99, 3);
echo "\nTotal: $" . $total;

// Modern PHP 8+ features
$items = ['apple', 'banana', 'cherry'];
array_map(fn($item) => strtoupper($item), $items); // arrow function

$data = ['name' => 'John', 'age' => 30];
$data['country'] ??= 'Unknown'; // null coalescing assignment

?>