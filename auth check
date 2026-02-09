// auth-check.js
document.addEventListener('DOMContentLoaded', function() {
    // Проверяем, авторизован ли пользователь
    const isAuthenticated = localStorage.getItem('isAuthenticated');
    
    // Если пользователь НЕ авторизован и НЕ на странице входа
    if (!isAuthenticated && !window.location.pathname.endsWith('login.html')) {
        // Сохраняем текущую страницу для редиректа после входа
        localStorage.setItem('redirectAfterLogin', window.location.pathname);
        
        // Перенаправляем на страницу входа
        window.location.href = '/login.html';
    }
    
    // Если пользователь авторизован и на странице входа
    if (isAuthenticated && window.location.pathname.endsWith('login.html')) {
        // Перенаправляем на главную
        window.location.href = '/index.html';
    }
});
