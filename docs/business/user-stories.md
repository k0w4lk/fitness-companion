
### User  


### Client  
**US-2:** "As a client, I want to search for trainers using different criteria with saved search parameters to quickly find a suitable specialist without re-entering data"  

#### Acceptance Criteria:  
**1. Search Filters**  
- [MVP] Specializations:  
  - Predefined list (yoga, crossfit, stretching)  
  - Manual tag input field  
- [ ] Rating:  
  - Slider (1-5 stars)  
  - 0.5 increments  
- [ ] Price range:  
  - 0 to 250 BYN  
  - 5 BYN increments  
- [ ] Location:  
  - Online/Offline toggle  
  - City dropdown (for offline)  

**2. Results Display**  
- [MVP] Pagination:  
  - 10 trainers/page  
  - "Show more" button  
- [ ] Default sorting:  
  - Rating (high → low)  
- [ ] Persistent filters:  
  - Survives profile navigation  
  - Saved in localStorage  

**3. Edge Cases**  
- [MVP] Empty results:  
  - "No matches found" message  
  - Filter reset option  
- [ ] Interactive hints:  
  - Tooltips (e.g., "Rating based on 20+ reviews")  

2. "Как клиент, я хочу:"
   - Видеть свободные слоты в календаре тренера
   - Бронировать тренировку с оплатой онлайн
   - Отменить бронь за 24 часа (автовозврат)

### Тренер:
1. "Как тренер, я хочу:"
   - Указывать свои специализации (выбор из списка + свои теги)
   - Управлять расписанием (блокировать дни, добавлять слоты)
   - Получать уведомления о новых бронированиях

### Общее:
1. "Как пользователь, я хочу:"
   - Общаться в чате (текст + файлы)
   - Оставлять отзыв после тренировки

2. "Как пользователь, я хочу ставить оценки другим пользователям"
   - Тренер может ставить оценки клиентам
   - Клиент может ставить оценки тренерам
   - Рейтинг рассчитывается как среднее арифметическое из всех оценок

3. "Как пользователь, я хочу иметь чат с другими пользователями"
   - В чате можно отправлять видео/документы
   - В чате сохраняется история сообщений

### Оплата:
1. "Как админ я хочу получать комиссию сервиса:"
   - С каждой оплаты взимать 10%
   - Иметь бонусную программу для уменьшения размера комисси до 5%
   - При отмене занятия взимать 15% с клиента и часть (до 10%) отдавать тренеру в зависимости от времени оставшегося до начала занятия. Оставшиеся средства возращаются клиенту
