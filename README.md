# To-Do List

## EN

### Business Requirements for a To-Do List Website

1. **Main goals of the Project**
    - **Providing a Task Management Tool**: After logging in, users should have access to an interface that allows them to create, edit, mark as completed, and delete tasks.
    - **Managing Recurring and One-Time Tasks**: Users should be able to specify whether a task is one-time or recurring and set the frequency for repeating tasks.
    - **Task Personalization with Tags**: Users can add tags to tasks, allowing easy grouping and filtering.
    - **Deadline Management**: Users can set task deadlines and decide whether to reschedule the task if it’s not completed on time.

2. **Users and Authentication**
    - **User Registration and Login**: The website must have a registration and login system that allows users to access their task lists.
    - **User Data Storage**: User data (such as passwords) must be securely stored and encrypted.
    - **Password Reset**: Users should have the option to reset their password if forgotten.

3. **Core Features**
    - **Task Creation**: Users can add new tasks with the following options:
        - Task Name
        - Task Description (optional)
        - Tag Assignment
        - Setting the task as one-time or recurring
        - Setting a deadline (or no deadline)
    - **Task Editing**: Users can edit existing tasks.
    - **Marking Tasks as Completed**: Users can mark tasks as completed, which will move them to the task history.
    - **Task Deletion**: Users can delete tasks they no longer need.
    - **Task Filtering and Sorting**: Users can filter and sort tasks by tags, date, or status (completed/incomplete).
    - **Task Tagging**: Users can assign tags to tasks for better organization.
    - **Managing Task Recurrence**: For recurring tasks, users can specify how often the task should repeat (daily, weekly, monthly, etc.).
    - **Deadline Management**:
        - Task without a deadline: The task will remain visible until it is marked as completed.
        - Task with a deadline: If the deadline passes, the user will be prompted to reschedule the task or mark it as completed.

4. **Notifications and Reminders**
    - **Email Notifications**: Users can receive reminders about upcoming tasks via email.
    - **Internal Notifications**: Notifications on the site about upcoming tasks, tasks to be rescheduled, or tasks that were not completed on time.

5. **Task History**
    - **Task Archiving**: After marking a task as completed, it should be moved to the "History" section, where users can review their completed tasks.
    - **Restoring Tasks from History**: Users can restore tasks from the task history if needed.

6. **User Interface**
    - **Responsive Design**: The website should be responsive, providing users with a comfortable experience on various devices (computers, tablets, smartphones).
    - **Intuitive Interface**: The interface should be intuitive and easy to use, with clearly marked features and options.
    - **Task List View**: Users should have the option to choose the task list view, e.g., as a list, calendar, etc.
    - **Dark/Light Mode**: Ability to switch between dark and light mode for better user comfort.

7. **Security**
    - **Secure Data Storage**: All data must be stored securely with appropriate encryption mechanisms.
    - **Protection Against XSS/CSRF Attacks**: The site should be protected against common web application security threats.

8. **Technical Requirements**
    - **Using Symfony and PHP**: The application should be written in Symfony and PHP, following best practices and design patterns.
    - **Database**: The choice of database (e.g., MySQL, PostgreSQL) depends on the project requirements and available resources.
    - **API**: The possibility of extending the site’s functionality through an API for integration with other services or applications.

9. **Additional Features**
    - **Calendar Integration**: Ability to synchronize with external calendars (e.g., Google Calendar) for importing or exporting tasks.
    - **Task List Export**: Users should be able to export their tasks to a file (e.g., CSV, PDF).
    - **Task Sharing**: Ability to share tasks or entire lists with other users.

10. **Monitoring and Reporting**
    - **Task Completion Reports**: Ability to generate reports of completed tasks within a specific time frame.
    - **Productivity Statistics**: Users can view statistics on their productivity, such as the number of completed tasks, average completion time, etc.

---

## PL

### Wymagania biznesowe dla strony internetowej listy To-Do

1. **Główne cele projektu**
    - **Udostępnienie narzędzia do zarządzania zadaniami**: Użytkownik po zalogowaniu ma dostęp do interfejsu, który umożliwia tworzenie, edytowanie, oznaczanie jako ukończone, oraz usuwanie zadań.
    - **Zarządzanie zadaniami cyklicznymi i jednorazowymi**: Użytkownik ma możliwość określenia, czy zadanie jest jednorazowe, czy cykliczne, a także ustawienia częstotliwości powtarzania zadań.
    - **Personalizacja zadań za pomocą tagów**: Użytkownik może dodawać tagi do zadań, co umożliwia łatwe grupowanie i filtrowanie zadań.
    - **Zarządzanie terminami wykonania**: Użytkownik może ustawić datę wykonania zadania oraz decydować o przesunięciu terminu, jeśli zadanie nie zostanie ukończone na czas.

2. **Użytkownicy i autoryzacja**
    - **Rejestracja i logowanie użytkowników**: Strona musi posiadać system rejestracji i logowania, umożliwiający użytkownikom dostęp do ich list zadań.
    - **Przechowywanie danych użytkowników**: Dane użytkowników (takie jak hasła) muszą być bezpiecznie przechowywane i zaszyfrowane.
    - **Resetowanie hasła**: Użytkownicy powinni mieć możliwość resetowania hasła w przypadku jego zapomnienia.

3. **Funkcje główne**
    - **Tworzenie zadań**: Użytkownik może dodawać nowe zadania z następującymi opcjami:
        - Nazwa zadania
        - Opis zadania (opcjonalnie)
        - Przypisanie tagów
        - Ustawienie zadania jako jednorazowe lub cykliczne
        - Ustawienie daty wykonania (lub brak daty)
    - **Edytowanie zadań**: Użytkownik może edytować istniejące zadania.
    - **Oznaczanie zadań jako ukończone**: Użytkownik może oznaczyć zadania jako ukończone, co spowoduje ich przeniesienie do historii zadań.
    - **Usuwanie zadań**: Użytkownik może usunąć zadania, które nie są już potrzebne.
    - **Filtracja i sortowanie zadań**: Użytkownik może filtrować i sortować zadania według tagów, daty, czy statusu (ukończone/nieukończone).
    - **Tagowanie zadań**: Użytkownik może przypisywać tagi do zadań, co pozwala na ich lepszą organizację.
    - **Zarządzanie cyklicznością zadań**: W przypadku zadań cyklicznych, użytkownik może określić, jak często zadanie ma się powtarzać (codziennie, tygodniowo, miesięcznie, etc.).
    - **Zarządzanie terminami**:
        - Zadanie bez przypisanej daty: Zadanie będzie widoczne do momentu jego zaznaczenia jako ukończone.
        - Zadanie z przypisaną datą: W przypadku, gdy minie termin wykonania zadania, użytkownik zostanie poproszony o przesunięcie zadania na inny dzień lub oznaczenie go jako ukończone.

4. **Powiadomienia i przypomnienia**
    - **Powiadomienia e-mail**: Użytkownik może otrzymywać przypomnienia o nadchodzących zadaniach na e-mail.
    - **Powiadomienia wewnętrzne**: Powiadomienia na stronie o nadchodzących zadaniach, zadaniach do przełożenia, lub zadaniach, które nie zostały wykonane w terminie.

5. **Historia zadań**
    - **Archiwizacja zadań**: Po oznaczeniu zadania jako ukończone, powinno ono być przeniesione do sekcji "Historia", gdzie użytkownik może przeglądać swoje ukończone zadania.
    - **Przywracanie zadań z historii**: Użytkownik może przywrócić zadanie z historii zadań, jeśli zajdzie taka potrzeba.

6. **Interfejs użytkownika**
    - **Responsywny design**: Strona powinna być responsywna, zapewniając użytkownikowi komfortowe korzystanie z niej na różnych urządzeniach (komputery, tablety, smartfony).
    - **Intuicyjny interfejs**: Interfejs powinien być intuicyjny i łatwy w użyciu, z jasno oznaczonymi funkcjami i opcjami.
    - **Widok listy zadań**: Użytkownik powinien mieć możliwość wyboru widoku listy zadań, np. jako lista, kalendarz, etc.
    - **Tryb ciemny/jasny**: Możliwość wyboru trybu wyświetlania (ciemny/jasny) dla lepszego komfortu użytkownika.

7. **Bezpieczeństwo**
    - **Bezpieczne przechowywanie danych**: Wszystkie dane muszą być przechowywane w bezpieczny sposób, z odpowiednimi mechanizmami szyfrowania.
    - **Ochrona przed atakami XSS/CSRF**: Strona powinna być zabezpieczona przed typowymi zagrożeniami związanymi z bezpieczeństwem aplikacji webowych.

8. **Wymagania techniczne**
    - **Wykorzystanie Symfony i PHP**: Aplikacja powinna być napisana w Symfony i PHP, zgodnie z najlepszymi praktykami i wzorcami projektowymi.
    - **Baza danych**: Wybór bazy danych (np. MySQL, PostgreSQL) zależy od wymagań projektu i dostępnych zasobów.
    - **API**: Możliwość rozszerzenia funkcjonalności strony poprzez API do integracji z innymi usługami lub aplikacjami.

9. **Dodatkowe funkcjonalności**
    - **Integracja z kalendarzem**: Możliwość synchronizacji z zewnętrznymi kalendarzami (np. Google Calendar) w celu importowania lub eksportowania zadań.
    - **Eksport listy zadań**: Użytkownik powinien mieć możliwość eksportu swoich zadań do pliku (np. CSV, PDF).
    - **Współdzielenie zadań**: Możliwość współdzielenia zadań lub całych list z innymi użytkownikami.

10. **Monitoring i raportowanie**
    - **Raporty z wykonania zadań**: Możliwość generowania raportów z wykonanych zadań w określonym przedziale czasowym.
    - **Statystyki produktywności**: Użytkownik może przeglądać statystyki dotyczące swojej produktywności, np. liczba ukończonych zadań, średni czas realizacji, etc.
