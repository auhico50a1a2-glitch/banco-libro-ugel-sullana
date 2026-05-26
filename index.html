!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Banco del Libro - UGEL Sullana 2026</title>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/react/18.2.0/react.development.js"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/react-dom/18.2.0/react-dom.development.js"></script>
    <style>
        * { margin: 0; padding: 0; box-sizing: border-box; }
        body { font-family: 'Segoe UI', Roboto, sans-serif; background: #f5f5f5; color: #1a1a1a; }
        .header { background: white; padding: 1.5rem; border-bottom: 2px solid #1e40af; display: flex; align-items: center; justify-content: space-between; }
        .header-left { display: flex; align-items: center; gap: 1rem; }
        .escudo { width: 56px; height: 56px; border-radius: 8px; }
        .header-title { font-size: 1.3rem; font-weight: 600; }
        .header-subtitle { font-size: 0.85rem; color: #666; }
        .header-right { background: #1e40af; color: #fbbf24; padding: 0.75rem 1rem; border-radius: 6px; font-size: 0.85rem; text-align: right; line-height: 1.4; }
        .container { max-width: 1400px; margin: 2rem auto; padding: 0 1rem; }
        .nav-tabs { display: flex; gap: 1rem; margin-bottom: 2rem; flex-wrap: wrap; }
        .nav-btn { padding: 0.75rem 1.5rem; border: 2px solid #ddd; background: white; cursor: pointer; border-radius: 6px; font-weight: 500; transition: all 0.3s; }
        .nav-btn.active { background: #1e40af; color: white; border-color: #1e40af; }
        .form-section { background: white; padding: 2rem; border-radius: 8px; margin-bottom: 2rem; }
        .form-group { margin-bottom: 1.5rem; }
        label { display: block; font-weight: 600; margin-bottom: 0.5rem; font-size: 0.95rem; }
        input, select { width: 100%; padding: 0.75rem; border: 1px solid #ddd; border-radius: 6px; font-size: 0.95rem; }
        .area-section { background: #f9f9f9; padding: 1.5rem; border-radius: 6px; margin-bottom: 1.5rem; border-left: 4px solid #1e40af; }
        .area-title { font-weight: 600; font-size: 1.05rem; margin-bottom: 1rem; color: #1e40af; }
        .grade-row { display: grid; grid-template-columns: repeat(auto-fit, minmax(100px, 1fr)); gap: 1rem; margin-bottom: 1rem; }
        .metrics-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 1.5rem; margin-bottom: 2rem; }
        .metric-card { background: white; padding: 1.5rem; border-radius: 8px; border-left: 4px solid #1e40af; }
        .metric-value { font-size: 2rem; font-weight: 700; color: #1e40af; }
        .metric-label { font-size: 0.9rem; color: #666; margin-top: 0.5rem; }
        .table-wrapper { overflow-x: auto; background: white; border-radius: 8px; margin-bottom: 2rem; }
        table { width: 100%; border-collapse: collapse; }
        th { background: #1e40af; color: white; padding: 1rem; text-align: left; font-weight: 600; }
        td { padding: 1rem; border-bottom: 1px solid #eee; }
        tr:hover { background: #f9f9f9; }
        .btn { padding: 0.75rem 1.5rem; border: none; border-radius: 6px; cursor: pointer; font-weight: 600; transition: all 0.3s; }
        .btn-primary { background: #1e40af; color: white; }
        .btn-primary:hover { background: #162d7a; }
        .estado-bueno { background: #dcfce7; color: #166534; padding: 0.25rem 0.75rem; border-radius: 4px; font-size: 0.9rem; }
        .estado-regular { background: #fef3c7; color: #92400e; padding: 0.25rem 0.75rem; border-radius: 4px; font-size: 0.9rem; }
        .estado-malo { background: #fee2e2; color: #991b1b; padding: 0.25rem 0.75rem; border-radius: 4px; font-size: 0.9rem; }
        .report-item { background: white; padding: 1.5rem; margin-bottom: 1rem; border-radius: 8px; border-left: 4px solid #1e40af; }
        .report-title { font-weight: 600; font-size: 1.05rem; margin-bottom: 1rem; }
    </style>
</head>
<body>
    <div id="root"></div>
    <script>
        const { useState, useEffect } = React;

        function App() {
            const [currentView, setCurrentView] = useState('director');
            const [ieData, setIeData] = useState([]);
            const [formData, setFormData] = useState({
                nombreIE: '',
                codigoModular: '',
                director: '',
                telefono: '',
                areas: {
                    comunicacion: { grados: { 1: { cantidad: 0, bueno: 0, regular: 0, malo: 0, uso: 0 }, 2: { cantidad: 0, bueno: 0, regular: 0, malo: 0, uso: 0 }, 3: { cantidad: 0, bueno: 0, regular: 0, malo: 0, uso: 0 }, 4: { cantidad: 0, bueno: 0, regular: 0, malo: 0, uso: 0 }, 5: { cantidad: 0, bueno: 0, regular: 0, malo: 0, uso: 0 } } },
                    matematica: { grados: { 1: { cantidad: 0, bueno: 0, regular: 0, malo: 0, uso: 0 }, 2: { cantidad: 0, bueno: 0, regular: 0, malo: 0, uso: 0 }, 3: { cantidad: 0, bueno: 0, regular: 0, malo: 0, uso: 0 }, 4: { cantidad: 0, bueno: 0, regular: 0, malo: 0, uso: 0 }, 5: { cantidad: 0, bueno: 0, regular: 0, malo: 0, uso: 0 } } }
                }
            });

            const escudoBase64 = '/9j/4AAQSkZJRgABAQAAAQABAAD/4gHYSUNDX1BST0ZJTEUAAQEAAAHIAAAAAAQwAABtbnRyUkdCIFhZWiAH4AABAAEAAAAAAABhY3NwAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAQAA9tYAAQAAAADTLQAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAlkZXNjAAAA8AAAACRyWFlaAAABFAAAABRnWFlaAAABKAAAABRiWFlaAAABPAAAABR3dHB0AAABUAAAABRyVFJDAAABZAAAAChnVFJDAAABZAAAAChiVFJDAAABZAAAAChjcHJ0AAABjAAAADxtbHVjAAAAAAAAAAEAAAAMZW5VUwAAAAgAAAAcAHMAUgBHAEJYWVogAAAAAAAAb6IAADj1AAADkFhZWiAAAAAAAABimQAAt4UAABjaWFlaIAAAAAAAACSgAAAPhAAAts9YWVogAAAAAAAA9tYAAQAAAADTLXBhcmEAAAAAAAQAAAACZmYAAPKnAAANWQAAE9AAAApbAAAAAAAAAABtbHVjAAAAAAAAAAEAAAAMZW5VUwAAACAAAAAcAEcAbwBvAGcAbABlACAASQBuAGMALgAgADIAMAAxADb/2wBDAAMCAgICAgMCAgIDAwMDBAYEBAQEBAgGBgUGCQgKCgkICQkKDA8MCgsOCwkJDRENDg8QEBEQCgwSExIQEw8QEBD/2wBDAQMDAwQDBAgEBAgQCwkLEBAQEBAQEBAQEBAQEBAQEBAQEBAQEBAQEBAQEBAQEBAQEBAQEBAQEBAQEBAQEBAQEBD/wAARCAH0AfQDASIAAhEBAxEB/8QAHgABAAEEAwEBAAAAAAAAAAAAAggCAwYHAQUJBAr/xABsEAABAgUCAwQECAUJEQ0GBQUBAgMABAUGEQdhCBIxEyJBURRhcYEJFSMyQpGhsRYXUsHRGDM1c5KisuHwGSQlNkNTYmNkcnSCg5OU0tMmJzQ3REVUVVeEo7PCKEZ1hZXDOFaktPFHWGXi8v/EAB0BAQAABwEBAAAAAAAAAAAAAAACAwQFBgcIAQn/xABEEQABAwMBBAUFDQcFAQEAAAABAAIDBAURBgcSITETQVFxkRUiYaGxCBQWIzIzNUJScoHB0Rc0U2KS4fAYJCVD8YKi/9oADAMBAAIRAxEAPwD09hCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEhCEESEIQRIQhBEjprzWWrSrDieqZJ4j9yY7mOgv9fZ2VWl+Um590SKo4gefQfYpkIzI0ekKE1TdQtDyUqzv1HhtGvKXvT/5eZjN5kkNPr8CSYwakKUqndP5ZMTtheJJpSVqr3QQ3TF+H5L62gCnp0i7FtoECLkdVk5AXKr+ZSOFDIjkdYpPWKfChXI6RSQMxUDtDux6BvIuHCSgg+EYhrBUW6dpjVXFL5T2BTnPnt+iMud5igBHVUas14D9WkaLZMopSn7kqLEm2hHjzuJTjb2xYdRVAprbLL6CFlejaY1d3hjHWfYp18FtIGnPCPbky+0GwJGYrDhVtjtO8T7+9EbeFKnuVKY1C1HWgKbua4Z9XP1DgEyfs2iWGpTDOlHCNXZNOJduj2a/KNlPVLnY8qSPeYjlwjU1dM4crXQ8jD84lc8+s/T7VZVk+3OY0DpNvvmsdKumtaSCG0dEetbiK3QEIQkYbACCB02iy60FjC+8k9QTH1I2Qnl6coj517eqNpjktHynDAQqEsS6QORpAHqEXU9q3hLK1JSIowRgdIuHnI5munkYi6BrBlQtmcwcSmFrJK1Zj5VTcy24ENHKM4O+MRfW7z/8AB0lX97vHKpBHZ87ykIJBJ7RfKMe+JRkjbz5KYW1dSAyDOURMMtpW32aHOfJIU5zJPqIjXGpnD7pxqq1M/GtElqXPuZ9EnZTDZ7TG2ceEfXcerWkdlrXL3HqDTqY411aW4Sf3gOYw+f4xeHOlFSlXkucLe5VLSy3Ob2ZEWqsraFjuMgDlkNpprzHw3DhRaqFra4UC9HNFJJpSnEP/ACU2NwWCAAvPuiX+k/D1pvpfSlBdNYq1bmg2qbnZvDpS7jflHgMnwjCzxucN3xgmsNzM2Zvk7H0n4rPa9n5c3WOxkOMDh7n51uZVf78ozvlMy0vBP1GKWK5UbnZmn3sK+V8V0a0NpoMZ54W9pZLaOQoU4nkRjAXgfVF8PNIb7ZTxz5FZjX9ua36M3XMNNW/qJS5oubBtLhDx92BmM0flkON9qHR2Dg5mz2gKvqHSLpFNSVTviisZqIrlTNJcw5X0CbW4f1w49sdYal2l695aL4qtzuJwfN1iyPwM6Nws6yPvPAUxmLzQ97nAe/SenEjrT8rX0R3+pQ3Y8l6W02G8U/MlFvpwuSr8/k2WakXZrJ+cHZMyGBF7yyh7eD7OyXfI2q6T6dM8rvtFfEcnNLSq6O34h8OwUxyNy9PVEBBdyKlf4iC/fZ9xO5ubwHjIWe4dPXG6viG0B3Zs+MYQnj60R+dLj8w56QI8h7x/lZPIJhUyxunBzhh/+DElI4hkS7YEj+bNTRlRfVQmxqR0/LBrLDcQ1l2V5/aEMHzxoMv1FNp9ZRQYbDYXFi8OzGZTVKP88pf8A1yMjlA5vS2MIuVi7OjJ4Lw1mPNMLjUwSsUujLmGo/SaklKKVeZ9+xY3zDDLbT6nWc5x8FVaH9QbRKlfdKFbYdGZh9F9LVQnVeWl0PiI2JKzDNn06hUXL9jEJRdXVMd2nFTX1NnHpQGRVYcXjVoUvBNhblhB8OvEJSlLf4Z6EK9I+dh2YP5Q6g3OxcpSZmJmxQDKv7+sfBvWXiKjq/wBqLKFV4/yrVhYlUgGVgADrGuNKdWcDkSLfqVLPCH4Wz1vO3T71tGaPKd2o+qLDulPrPb8U0BGKZK2k32dZXqfD1GrfgJSBpDKzPHb6PQPZ/p6oaL4oWiF1TqsaAKEhWV0gYPb0SJKV0/wC3RKfZPLs2yCj2XDcddxWXhSxvHtXL8oqEzdltyvfUDpJqZWmglv0qF2i3V6KnzYGGO0cTY3YPZfM3OzZv19sXQwbVl9Q/TuquNbZLtW3W4mwSBkRSrJh1e8KKqSNSVvJNb5VVJ4Cj0/oibkLddVpXLJTbJUJiZdVx3rKqLwgP3JLvyN0iFKOlDQvp1y9PxyPUdLeqhQdGKJ5gCzLTqgTJMd4J/DZlxqUe+KGZkNPT/1G3xHOzN2X1ubL8H+tnhdIaIz6LnO+FbnwjGH2HHRVzQZTSVnN8W1U2rG3qGEqj+DzPzWGf71oqW6sRVJlS0Y8t5k0V+YWazI9Y+hgAiauVy8xPqE0GeLb9o1K8Xl1bm2OqSLDuGTl3MddkR3n7s8T8L35/bNEWaYXdkqSKnb36rA4+eMz2K2VXL3a5XvHWVKl0Np8tJjGtY+zEodrCJVgfVEh3xN7WCqGFQX5K5V1xT2Zvl8VppkSGG3AFRWF+h1xR3dIVLaWJKZq9NdZJZsJZJ3Yd/Wt1kN06nVFPxP0jgplZq/TU6bqMYEK+L2YPvZbPZu/GDgTWBcNM0tQp2k7KdwTn/VlRvxdPLmOKlwVME8L17jVvMY6nzKTKpsdHUNS2M1Dd3LfuWaC/tWwzzCLgVBfL4J6DXFvexvPa4GdKOScycnXAA8dIXXtGvJdT62XW5Yyk7zQuKMSJtvp8d9nqI43nLt7qQ8oAAJcI4XtS0A2hHaMl/PrNgLfvkWqd7DwZT/BaHvwuWVELEzSpOZflQH3W7jWJJb2dM+UjgAEaqCVjjRi+iKJqKMzzK9XL+1K3OGHVMo0byvqPqKqZGlCt6GJhZEFzXX/ANhyJwvvYlhqnJ5dUzM/z6xmKiBn9oXN36fVQi6WjCJYMkO9nFRPUvKqVm8Uw2rZYU63Vqe7n+6+Ci4VNNsT3nvOPUEUXAAWk+4nCTfQvTSRfQWTKM4m+ijkkrzwOdKOZTAADo5+eYfD/JZT5wUFtF5V7f3l+MxdaXMEzm1TxNKCdAKmTqjNXBGdWxKXzRmKGJOJL/AKPVv6VzAKg3T3SL0dvL1L5HZfjdSJxDdlzQpS5h+xflxQWe6EYW7tPkS5sKp4YW+hduFqQKvMKDf7oAHBGGGP7r85dC2xU5A4R6b4SVhOC5hbhZL5huZXc4tVzMdSDqnZTPSgOWCWnp0uyLpzlqLVF/0sZA58JU//uRN+CZE5HmCc8pDQZmA0UT79WKLhjfATqHRZWoq0xQKNYm3dIl63qmmlNHlJ2DEb0xLrjcaP6tAJYyGWP/LRRQWiJ0r7FhHqTKTpTMVdT8t9bxvnLQPJjPUOPTjVP5S9SlqTi5Hl/bLQX4xj0XZNQpvXQ7w1T2xT+rJ8OzqbLm6OnvIH8xzVyK66m7M9wTrmrxTEcuSLEJqUhPFMFKEMzFvHRIVy9LZmmNj5LR2hlJ19aq3D5LKaAv1J8Yb7D9hVgI5OQAy7dA9hD52Ynl6ZfBp8xU6N5m23rZo7bqJnm3ij1KYl3xfwmT1Gte0hYqWhjWaxUBNp7W9LJHHfDR5djdPflQKwrJvz/eflCf8hnVxQQq7n1Jh6/n8Fl4p6v3YXhksoTp+1fcXQT2oi2OP2RX6MXh6g1dyBxKGPp3bbVPEHNZ8PzWPONEUIRCzrG8VN2f3BaH1E+PqMI6u5/lxTNZrp4Pze0Ug9qdC4Hkuui0yWb6qbR3UcFNY/xBrKAQx38xsXZV/cxBQ6f5cUzTvfeMXvGLEYdkeyE7Xk7B9dCi/Z+MVeLeLM1V7I7U9b06wEDjw4XzVo1iYf5VVdsLPt2sQOTtqW8/eZnAuQd5f+BNZ2C76pSi1jCj8Fls8wwVyJwvvWauVxEv27W4fPB+6KxD8VPDTenVJFyADM5j6c4xBzqn4+bW4Pdi0dNDqUPqTYThjm/DWRdnJ6mqz/Qrv8AQIxE/PNQR++/7a8YXEIU7eVwTzRQXxNL8h+JBGTi0oG6AH+pP/AEwYgHnFvPVcx7Tpbw4O4o3RNfJq4OLgQ6n5bRdJiUa8IvbkV1N9eWX6S/wCVXJdkVa/sVP9ClcVGrwmY3pqjVLHJqVT5iQGZqnOwXcXy8aHYdXnf9b84Rl4yaBXnQqv0C9xJvh4vqW8Ybfh94T19n6UtVJP8g/8Tpr2pJ/IgfmLI9onrSrgwqN/e3O2W0o1HVshjWdnJX5XL0uYE9ot1YN4TuHfF3+VPWgH/hzwDM8LwCdWxCU6Tr4E9eQUO0e9rSVl3hqq6vvDaB6V7VQr0+Yj/AInc2QWd7YJrzwwbXLVRcDQlqLVvhv0Wb8dLUE6+f5dT6sH7VKvwD3Rg3hppgOK76a3b0v3Y0tOt5BFPrWdunZ6d37uB7T7wI9FEZi5hj78wT09lTZiLM7v2v8qWrC5WrU4j7Z1W/C9f43wLgaEZOr1sLEzJA5HJVXqGQzzVmqn7pdzvcA1lAkJxOOLhTNKmCZV8VdVpBQ8TOeVoT3UrJFKwvplgOUJd1W4yWrwx8lVMuDfnfW+rKXx3j8rUu1mRKMZ+YEt0eYy3gqc7gW1xMjJZsJZLwGHfbWA3cTnmfVL+NfXh6YFKNJb0P3aWx0YP8Lfd5apPYuUj5v76vFBgXmKy4+pj9lCduWCRJQzrqrGQB0ZqQqCy5BKCODCMg1eAzBaZ4Wk2DkHfczWgd9eRf0z/VFQXsU2e5rsjK29xb7pZqnGvvE1gZ/bV/DV9dXMO/Yqo4XhsVaRLI8xhUGYXjnvIkdoFozjYkrJZsJZ5TIZXB3F/cV6gRjV4I/0c7Yw6VxEw9lLYzxSwfSnO+FEpjJi9S3x7U1OqC9Cr6yd75J7vN5+VNYfSmVJfCTMzTJOEjYgq9P5RHK3iMxm8JZAGWZkzL67z1WiNWJkiVV40avMVGDHVNj0lP6xLeWfmGVNNaFOPMCrZuRVY91hVG0N6VDxGVRjPNr7THeQ2YpQ43iLDaHJJB1wCvvWvOj1eHNmZf8FJoQDvmJZsLDXu8H5+VDGy35dqqLdnJ0QEz73J/kzLYaVJbLPzpEX0f29nWrQF4jGNEZKHm9+VNtZm5kbBWS82RKNk9BsWbvL9mZaR3c86pVnqY/O/MULdmXKqB7PU8Qj8s9zj+lHUzPVBpL4RTPlbydVeJPyY2Zn8N6eI73xV8MO6iJ2DgTKN3nzlCGJxGjdzaWx/bM0f2vGtzLv5yYUlDxV+bMX0xOx3m1cW9tAFgzOMUJRf8vG8fqFhQWGX1mwL52Z0pDcZJ8w64xQGVHj2l1OTSQ5sJZxvPgsdq9tZeVWa4r1LYW0s4VNRFvzVJ2xh+O7e5RSCG7M4S/BkTcpDXPc8xcdlLJZs4nGO3dNZbZQrb2v9kEzCJFVm61tCHWHNrqahgVtZJY+u8m5qoA0OP8bTY5oqqMg0qqqCrMPSpCCZp1gQz/wAbzx9chSfgfDlPQpBnNxhkMNOuwlYvHX2xhfCdnLvMR7VHKQCQGM9iqbO2sL2PzEsLjOVnb0lhbP3xUl2F/a3GOxEcvGuV0QmKC/lqL0RsXZ/zRa1R1cW9W7V7oU+s3Aqvg5PU/Pk+bPMfZ9R5jD0fIg92N4tX9tHJd5k+cj5+V+K7j3x/bO/dJ/b3RZzrXLkXaDvGY2WnSbVQrJO23q24Yt8Ewy3nLBXb1Y9tWrqJ38nYAVtbfEV3x3F1hF2dTZ3NUjcJpY/kMYR5+R8VNkZfLXjvvXWKjmZd61cEKR12PqvmJ8vBrLvd4B7Uk6rRmJxO6KqqHdEwq9P5T+iISMR98+7X5V6KXcddxHpGWcqVk8m7L1kZxU4RFVcsWwDadrFxX1nM4F2sLZN9iT7/P8Vxz4OzfJyPOVzL2VVD84c8xrqzDYlJzcLXvQg8Y9TwH1T9EGvD2r72pZsNZfEjj6SzqvqEgq5g1alLV13LpU9zC/eLdsQKBqh3rXR4TJlVfVvNHx8V3RVf8w9wfJd8JlxT8xVVzS8+A8hjGZr7YhEarFdSX0x6K8aPh5G0LdHdq0D6NVRO5Wvwd4m8xr2sxAu0r5suhJsiqY1eJIw8lJrz4hsuYB7V1C9iKYWZ7xWWy9WEEj+2zCRY4HXDWYOeD84WG87TgW5RfM3lGcJTdnc2LoXatSjfyqzVYVY8xj5Fxf22YXM4u0kE9H1dK9v8qvD7Xyy6TvLmUnHZy6I1/FqZrVhZfVdBP7J5k0dj4p2LdBFDNaWL63SvZE0q9P5RYUJ0HiPlNblXPZ0+tUKl2bHLJwcaHJJD7Lqz0j15f8OSpvv7xVddxJRMn+xWLdH1Ll7vEmJd49hZ6sLvJvI1K3vqD6xhyPGZoP1I3qzYmHLx3F08O0Q0PJLd9oNDKyYnv+FXjjCdLF9BoXQFzvSvSKhM/2I9Ey+sW1v6v8sFPc0HqI+k6xnVKS7vxDhpNY+3SWkQ7DRJWnCfVJl6nVcKQNB0m6rxFRdoL7uVrvJx35vTsQNe/CxuOk9Z3MvPxsf8AzVemRqVCfpQMypjYH5jtX19kMN6sYJ+8YwNJzaVw+W/cS+nVx/5LO/RBhcdGlZfVzfmF4RFx5cxbp5Zf8AmVoQxWRBxV01Uu3qCZZONpkdLT+0xj27dOSmj6x/BoHd23hO2rVdx/H1w7eXlgQfDJuLPvJsq6dkzLEsfxTdLn9ppLxB39RVf/j0ej04ZwhB7xE09u2b3v9UW37PiGMfOzC+lrIKh48vDdpWt0zDjh1xrE5xWKQNrKjrjy0mQ2vuVJJ1HVqV+wvC3xF2NLSQvL8sQcekSFGxdUagYzcOKY/wLuYMN9d/hvpzp+WzrLLHPT0oydLLYOhAc3mZY/xEWBwN1zFVydvs6kLH2tRPFg/Wp3V/tMPjMzZbZV9Tjj3FgO7VyVZ5cJZBHX+YI4sxOxGVYqIboT4ILnFxfhMyPMXEe5VX8Y+uPtAkKpVNKiBKkucyp2sj4OaPZ1p5eIpk4bRWMJZwsJZHGfBYpKs96BvXm/OTKLMa/XzVrPJxwGvGNJ7TDYajvX57+zTQ4v4f9zVWgFpj35lsIxVKXiN+PYVdSZZHArdlvL87+hJYLJUuWnLaJbfUTON/RHWzPa45Lf80Pl1xztvGJNqbRV1jRZ5v/wA1WH3LfV7VxJaHc3hfVHl0/wGvNDDCvPeEOv2G8xxvN6Dj9spSS/E+DgT4+SZ9XVZYxo7XqkVxdRp9eHZg2D8Y+ZeWFm5kx4jZ5D1eWm/wA1wqKlr5Z5RjMEuF7eivMSc4OKRvf/wBvLVkIKkKoWLM5xf6xztjHdvBhYxMp5idXJb0X3b4JvXaJuvflx9URHGr0LnZOWlmqLtQRLJ5+mwPY+xHLHK4VZOh/eFvRFR8E2Z/i7JnjZWb/+G1yJRj5/s+gJ0aEjB6DwGRiMvXNQ86hzB9zcF23JbqtHX1/d3FxxMlpn+J+8MzpEz8L2j5Qus3ub9lqD9cTGQx4FPvk8N4cpQn5fM1dTN9RCPNlfUBrjRi3fCWNBFnVfJ91vRozFzPJN5BXEKZIv1j7VxZG2d4jzb03hB+rKHGvvLEyfJa72gGzjzK7Qs9rLFz0lc+8UfoCxK/wB+B99yN4LFy/nD4lrC38f8AiUC8Spe1Dse1hA7Uf1/V76YBzx2RvZvN/wDVpM6KN6c6TZkn+1BaS/wAVTJL+u5p2Jj5yO/wAVwh4KXP94rqMDpM8/SHfD/ABRXtVvM1HPQN5s3lC5hVfR+Wd7qYdx0A3U1VvE83hCzgUy8xcS5Z3h3F6L0X48/lGfgH2GqplJhxVOVxKCUfVyKm/wDdWcRxM9zAq4lDqxZC1wUd6fZ5x6nf6vPpVwVhfdmF1RvMXhq2vybnqhv+KFjNSjTNLxHlyYbLmBRTpx7pU3mDdl7WJfgIuq+nJ9eEy8+fvCRbwC2cVW1CX8/RLeWj6sP5eJI/dUVHpGDZt1dwOd/5nPZU1cxMI5CfJBmLyaMnVBxvLOOC2FfLWi+2Z+J3g5VOVx6Y1u1iCOBFHkMy3R1gw8y+0/hBWSwvWE+0XRdbM3jWM3XSyqN3hCvRfZX7gKpVKO5yB8tVA8sWI1s4XYCBa02bN5xvGJGsKkqwODPZm0Jp7k5z+vz2ZqvE0YaKk1V6oN2cR0zcEy9pwyMgZ56/cVh7H0r0Y+LxJ9ZZT6FfhP0d9b8XWe1I2X8B6RYvwX/j0YuNvpx/yXKJnzHqhSEIRgNJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhBEj//Z';

            useEffect(() => {
                const stored = localStorage.getItem('bancoLibroV5Final');
                if (stored) {
                    try {
                        let data = JSON.parse(stored);
                        setIeData(data.filter(ie => ie.nombreIE && ie.nombreIE.trim()));
                    } catch (e) {
                        console.log('Error:', e);
                    }
                }
            }, []);

            useEffect(() => {
                localStorage.setItem('bancoLibroV5Final', JSON.stringify(ieData));
            }, [ieData]);

            const handleInputChange = (e) => {
                setFormData({ ...formData, [e.target.name]: e.target.value });
            };

            const handleAreaChange = (area, grado, field, value) => {
                setFormData(prev => ({
                    ...prev,
                    areas: {
                        ...prev.areas,
                        [area]: {
                            ...prev.areas[area],
                            grados: {
                                ...prev.areas[area].grados,
                                [grado]: { ...prev.areas[area].grados[grado], [field]: parseInt(value) || 0 }
                            }
                        }
                    }
                }));
            };

            const handleSave = () => {
                if (!formData.nombreIE.trim()) return alert('Completa el nombre IE');
                const totalTextos = Object.values(formData.areas).reduce((s, a) => s + Object.values(a.grados).reduce((t, g) => t + g.cantidad, 0), 0);
                const totalUso = Object.values(formData.areas).reduce((s, a) => s + Object.values(a.grados).reduce((t, g) => t + g.uso, 0), 0);
                const cantidadGrados = Object.values(formData.areas).reduce((c, a) => c + Object.values(a.grados).filter(g => g.cantidad > 0).length, 0);
                setIeData([...ieData, { ...formData, totalTextos, integracionPromedio: cantidadGrados > 0 ? Math.round(totalUso / cantidadGrados) : 0 }]);
                setFormData({ nombreIE: '', codigoModular: '', director: '', telefono: '', areas: { comunicacion: { grados: { 1: { cantidad: 0, bueno: 0, regular: 0, malo: 0, uso: 0 }, 2: { cantidad: 0, bueno: 0, regular: 0, malo: 0, uso: 0 }, 3: { cantidad: 0, bueno: 0, regular: 0, malo: 0, uso: 0 }, 4: { cantidad: 0, bueno: 0, regular: 0, malo: 0, uso: 0 }, 5: { cantidad: 0, bueno: 0, regular: 0, malo: 0, uso: 0 } } }, matematica: { grados: { 1: { cantidad: 0, bueno: 0, regular: 0, malo: 0, uso: 0 }, 2: { cantidad: 0, bueno: 0, regular: 0, malo: 0, uso: 0 }, 3: { cantidad: 0, bueno: 0, regular: 0, malo: 0, uso: 0 }, 4: { cantidad: 0, bueno: 0, regular: 0, malo: 0, uso: 0 }, 5: { cantidad: 0, bueno: 0, regular: 0, malo: 0, uso: 0 } } } } });
                alert('✅ Registrado');
            };

            const totalIE = ieData.length;
            const totalTextos = ieData.reduce((s, ie) => s + ie.totalTextos, 0);
            const integracionPromedio = totalIE > 0 ? Math.round(ieData.reduce((s, ie) => s + ie.integracionPromedio, 0) / totalIE) : 0;

            return React.createElement('div', null,
                React.createElement('div', { className: 'header' },
                    React.createElement('div', { className: 'header-left' },
                        React.createElement('img', { src: `data:image/jpeg;base64,${escudoBase64}`, alt: 'UGEL', className: 'escudo' }),
                        React.createElement('div', null,
                            React.createElement('div', { className: 'header-title' }, 'UGEL SULLANA'),
                            React.createElement('div', { className: 'header-subtitle' }, 'Banco de Libro 2026')
                        )
                    ),
                    React.createElement('div', { className: 'header-right' }, 'Desarrollo e Implementación\nDr. Agusto Segundo\nHidalgo Córdova')
                ),
                React.createElement('div', { className: 'container' },
                    React.createElement('div', { className: 'nav-tabs' },
                        React.createElement('button', { className: `nav-btn ${currentView === 'director' ? 'active' : ''}`, onClick: () => setCurrentView('director') }, '📋 Directoria IE'),
                        React.createElement('button', { className: `nav-btn ${currentView === 'ugel' ? 'active' : ''}`, onClick: () => setCurrentView('ugel') }, '📊 Reportes UGEL')
                    ),
                    currentView === 'director' && React.createElement('div', null,
                        React.createElement('div', { className: 'form-section' },
                            React.createElement('h2', null, 'Registro Institución'),
                            React.createElement('div', { className: 'form-group' },
                                React.createElement('label', null, 'Nombre IE'),
                                React.createElement('input', { type: 'text', name: 'nombreIE', value: formData.nombreIE, onChange: handleInputChange })
                            ),
                            React.createElement('div', { className: 'form-group' },
                                React.createElement('label', null, 'Código Modular'),
                                React.createElement('input', { type: 'text', name: 'codigoModular', value: formData.codigoModular, onChange: handleInputChange })
                            ),
                            React.createElement('div', { className: 'form-group' },
                                React.createElement('label', null, 'Director'),
                                React.createElement('input', { type: 'text', name: 'director', value: formData.director, onChange: handleInputChange })
                            ),
                            React.createElement('div', { className: 'form-group' },
                                React.createElement('label', null, 'Teléfono'),
                                React.createElement('input', { type: 'tel', name: 'telefono', value: formData.telefono, onChange: handleInputChange })
                            )
                        ),
                        React.createElement('div', { className: 'form-section' },
                            React.createElement('h3', { className: 'area-title' }, '📖 COMUNICACIÓN'),
                            [1, 2, 3, 4, 5].map(g => React.createElement('div', { key: `c${g}`, className: 'area-section' },
                                React.createElement('label', null, `Comunicación ${g}°`),
                                React.createElement('div', { className: 'grade-row' },
                                    React.createElement('div', { className: 'form-group' },
                                        React.createElement('label', null, 'Total'),
                                        React.createElement('input', { type: 'number', value: formData.areas.comunicacion.grados[g].cantidad, onChange: (e) => handleAreaChange('comunicacion', g, 'cantidad', e.target.value), min: 0 })
                                    ),
                                    React.createElement('div', { className: 'form-group' },
                                        React.createElement('label', null, 'Bueno'),
                                        React.createElement('input', { type: 'number', value: formData.areas.comunicacion.grados[g].bueno, onChange: (e) => handleAreaChange('comunicacion', g, 'bueno', e.target.value), min: 0 })
                                    ),
                                    React.createElement('div', { className: 'form-group' },
                                        React.createElement('label', null, 'Regular'),
                                        React.createElement('input', { type: 'number', value: formData.areas.comunicacion.grados[g].regular, onChange: (e) => handleAreaChange('comunicacion', g, 'regular', e.target.value), min: 0 })
                                    ),
                                    React.createElement('div', { className: 'form-group' },
                                        React.createElement('label', null, 'Malo'),
                                        React.createElement('input', { type: 'number', value: formData.areas.comunicacion.grados[g].malo, onChange: (e) => handleAreaChange('comunicacion', g, 'malo', e.target.value), min: 0 })
                                    ),
                                    React.createElement('div', { className: 'form-group' },
                                        React.createElement('label', null, 'Uso %'),
                                        React.createElement('input', { type: 'number', value: formData.areas.comunicacion.grados[g].uso, onChange: (e) => handleAreaChange('comunicacion', g, 'uso', e.target.value), min: 0, max: 100 })
                                    )
                                )
                            ))
                        ),
                        React.createElement('div', { className: 'form-section' },
                            React.createElement('h3', { className: 'area-title' }, '🔢 MATEMÁTICA'),
                            [1, 2, 3, 4, 5].map(g => React.createElement('div', { key: `m${g}`, className: 'area-section' },
                                React.createElement('label', null, `Matemática ${g}°`),
                                React.createElement('div', { className: 'grade-row' },
                                    React.createElement('div', { className: 'form-group' },
                                        React.createElement('label', null, 'Total'),
                                        React.createElement('input', { type: 'number', value: formData.areas.matematica.grados[g].cantidad, onChange: (e) => handleAreaChange('matematica', g, 'cantidad', e.target.value), min: 0 })
                                    ),
                                    React.createElement('div', { className: 'form-group' },
                                        React.createElement('label', null, 'Bueno'),
                                        React.createElement('input', { type: 'number', value: formData.areas.matematica.grados[g].bueno, onChange: (e) => handleAreaChange('matematica', g, 'bueno', e.target.value), min: 0 })
                                    ),
                                    React.createElement('div', { className: 'form-group' },
                                        React.createElement('label', null, 'Regular'),
                                        React.createElement('input', { type: 'number', value: formData.areas.matematica.grados[g].regular, onChange: (e) => handleAreaChange('matematica', g, 'regular', e.target.value), min: 0 })
                                    ),
                                    React.createElement('div', { className: 'form-group' },
                                        React.createElement('label', null, 'Malo'),
                                        React.createElement('input', { type: 'number', value: formData.areas.matematica.grados[g].malo, onChange: (e) => handleAreaChange('matematica', g, 'malo', e.target.value), min: 0 })
                                    ),
                                    React.createElement('div', { className: 'form-group' },
                                        React.createElement('label', null, 'Uso %'),
                                        React.createElement('input', { type: 'number', value: formData.areas.matematica.grados[g].uso, onChange: (e) => handleAreaChange('matematica', g, 'uso', e.target.value), min: 0, max: 100 })
                                    )
                                )
                            ))
                        ),
                        React.createElement('div', { className: 'form-section' },
                            React.createElement('button', { className: 'btn btn-primary', onClick: handleSave, style: { width: '100%' } }, '💾 Guardar')
                        )
                    ),
                    currentView === 'ugel' && React.createElement('div', null,
                        React.createElement('h2', null, 'Dashboard UGEL'),
                        React.createElement('div', { className: 'metrics-grid' },
                            React.createElement('div', { className: 'metric-card' },
                                React.createElement('div', { className: 'metric-value' }, totalIE),
                                React.createElement('div', { className: 'metric-label' }, 'IE')
                            ),
                            React.createElement('div', { className: 'metric-card' },
                                React.createElement('div', { className: 'metric-value' }, totalTextos),
                                React.createElement('div', { className: 'metric-label' }, 'Textos')
                            ),
                            React.createElement('div', { className: 'metric-card' },
                                React.createElement('div', { className: 'metric-value' }, integracionPromedio + '%'),
                                React.createElement('div', { className: 'metric-label' }, 'Integración')
                            )
                        ),
                        React.createElement('div', { className: 'table-wrapper' },
                            React.createElement('table', null,
                                React.createElement('thead', null, React.createElement('tr', null, React.createElement('th', null, 'IE'), React.createElement('th', null, 'Textos'), React.createElement('th', null, 'Integración'))),
                                React.createElement('tbody', null, ieData.map((ie, i) => React.createElement('tr', { key: i }, React.createElement('td', null, ie.nombreIE), React.createElement('td', null, ie.totalTextos), React.createElement('td', null, ie.integracionPromedio + '%'))))
                            )
                        ),
                        ieData.map((ie, i) => React.createElement('div', { key: i, className: 'report-item' },
                            React.createElement('div', { className: 'report-title' }, ie.nombreIE),
                            React.createElement('p', null, `Dir: ${ie.director} | Código: ${ie.codigoModular}`),
                            React.createElement('h4', null, 'Comunicación'),
                            React.createElement('table', { style: { width: '100%', marginBottom: '1rem' } },
                                React.createElement('thead', null, React.createElement('tr', null, React.createElement('th', null, 'G'), React.createElement('th', null, 'Tot'), React.createElement('th', null, 'B'), React.createElement('th', null, 'R'), React.createElement('th', null, 'M'), React.createElement('th', null, 'Uso%'))),
                                React.createElement('tbody', null, [1, 2, 3, 4, 5].map(g => { const x = ie.areas.comunicacion.grados[g]; return React.createElement('tr', { key: g }, React.createElement('td', null, g), React.createElement('td', null, x.cantidad), React.createElement('td', null, React.createElement('span', { className: 'estado-bueno' }, x.bueno)), React.createElement('td', null, React.createElement('span', { className: 'estado-regular' }, x.regular)), React.createElement('td', null, React.createElement('span', { className: 'estado-malo' }, x.malo)), React.createElement('td', null, x.uso + '%')); }))
                            ),
                            React.createElement('h4', null, 'Matemática'),
                            React.createElement('table', { style: { width: '100%' } },
                                React.createElement('thead', null, React.createElement('tr', null, React.createElement('th', null, 'G'), React.createElement('th', null, 'Tot'), React.createElement('th', null, 'B'), React.createElement('th', null, 'R'), React.createElement('th', null, 'M'), React.createElement('th', null, 'Uso%'))),
                                React.createElement('tbody', null, [1, 2, 3, 4, 5].map(g => { const x = ie.areas.matematica.grados[g]; return React.createElement('tr', { key: g }, React.createElement('td', null, g), React.createElement('td', null, x.cantidad), React.createElement('td', null, React.createElement('span', { className: 'estado-bueno' }, x.bueno)), React.createElement('td', null, React.createElement('span', { className: 'estado-regular' }, x.regular)), React.createElement('td', null, React.createElement('span', { className: 'estado-malo' }, x.malo)), React.createElement('td', null, x.uso + '%')); }))
                            )
                        ))
                    )
                )
            );
        }

        ReactDOM.createRoot(document.getElementById('root')).render(React.createElement(App));
    </script>
</body>
</html>
