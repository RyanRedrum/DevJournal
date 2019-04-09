# Dev Journal

## Wednesday April 03 2019
---


**Description**: Getting a date from a datetime in sql server.
https://stackoverflow.com/questions/113045/how-to-return-only-the-date-from-a-sql-server-datetime-datatype

```sql
SELECT CONVERT(date, getdate())
```

**Tags**: #tsql #date #datetime

---

**Description**: Resharper annoying on startup.  https://resharper-support.jetbrains.com/hc/en-us/community/posts/115000784870-How-do-I-turn-off-the-nagging-notifcation-Configure-settings-to-improve-performance


**Tags**: #resharper

---

## Thursday April 04 2019
---


**Description**: Select exists directly as a bit https://stackoverflow.com/questions/2759756/is-it-possible-to-select-exists-directly-as-a-bit

```sql
SELECT CAST(
   CASE WHEN EXISTS(SELECT * FROM theTable where theColumn like 'theValue%') THEN 1
   ELSE 0
   END
AS BIT)
```

**Tags**: #tsql #exists

---

## Monday April 08 2019
---


**Description**: Getting null default value from list of int https://stackoverflow.com/questions/1825304/return-null-for-firstordefault-on-empty-ienumerableint.

```csharp
int? nullableId = GetNonNullableInts().Cast<int?>().FirstOrDefault();
```

**Tags**: #csharp #nullable int

---

## Tuesday April 09 2019
---


**Description**: Android studio updates not running https://android.stackexchange.com/questions/55258/unable-to-install-system-images-for-the-android-sdk-failed-to-create-directory

Needed to run Android Studio as administrator.  Duh.


**Tags**: #AndroidStudio

---