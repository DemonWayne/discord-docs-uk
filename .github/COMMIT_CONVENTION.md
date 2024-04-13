## Git Commit Message Convention

> This is adapted from [Angular's commit convention](https://github.com/conventional-changelog/conventional-changelog/tree/master/packages/conventional-changelog-angular).

#### TL;DR:

Повідомлення має відповідати наступному регулярному запиту:

```js
/^(revert: )?(feat|fix|style|workflow|build|ci|chore|wip)(\(.+\))?: .{1,72}/;
```

#### Приклади

Ми додали новий файл "guild_create", тож використовуємо тег "feat" / Ми додали нову інформацію щодо того як працюють тайм-аути:

```
feat(guild_create): add general info about guild create
```

```
feat(timeout): update info about timeout work
```

Ми виправили якусь помилку в тексті з інформацією про зміну ролей, тож використовуємо тег "fix" (при наявності згадуйте проблему в описі):

```
fix(role_update): fix info about role deletion

close #12
```
### Повна форма повідомлення

Повідомлення коміту містить **хедер** (header), **тіло** (body) та **футер** (footer). Хедер містить **тип** (type), **розділ** (scope) та **тему** (subject).

```
<type>(<scope>): <subject>
<BLANK LINE>
<body>
<BLANK LINE>
<footer>
```

Хедер є обов'язковим, а розділ хедера необов'язковий.

### Розділ

Розділом може бути будь-що, дивлячись на місця зміни коміту. Для прикладу `guild_create`, `guild_roles_settings`, `guild_moderation` та інше...

### Тема

Тема містить стислий опис зміни:

- use the imperative, present tense: "change" not "changed" nor "changes"
- don't capitalize the first letter
- no dot (.) at the end
