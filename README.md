# chunks-of-my-code
Implemented tasks

Валідація форм твігу


html5 валідація працює для reqiured, то якщо поле required буде помилка, що його треба заповнити. Краще додавати form_errors для полів, що Не reqiured на випадок коли перевірки додадуться.
<div class="text-red-500 text-xs italic">
    {{ form_errors(form.registrationYear, {'attr': {'class': 'text-red text-xs italic'}}) }}
</div>

останній запис з бд
SELECT * FROM {table} ORDER BY {date_fileld} DESC LIMIT 1;

останній запис для якого треба знайти ще попередній (але якщо з годинами)
SELECT * FROM {table} WHERE {date_field} < {date} ORDER BY {date_fileld} DESC LIMIT 1;

роути в контролері по назві екшена будуються, тобто якщо в контролері екшн просто getAction, то роут буде такий як префікс '/chatbot/tracking' , якщо було б наприклад getTrackingAction то роут був би '/chatbot/tracking/tracking'
проблема в тому що для контролера стоїть префікс /chatbot/tracking
відповідно всі роути будуть починатись із /chatbot/tracking