#Третье задание для shri-2016. Ответы.

В тестировании спользовалась обычная консоль файрфокса и документация к ServiceWorker. Редактировался только worker.js.

1. Найдена ошибка с лишней точкой запятой в worker.js (найдено по сообщениям об ошибке, которые выдавала консоль).
2. Исправлены пути в urlsToCache в worker.js (найдено путем беглого просмотра кода).
3. worker.js был переложен в другую папку, уровнем выше (найдено, после изучения документации к ServiceWorker).
4. Список учеников не обновлялся из-за того, что в worker.js был использован Promise.race, то есть, часто возвращался старый кэш, а не обновленный, что быстрее выполнится. 

Дополнительные задания не сделаны. 
