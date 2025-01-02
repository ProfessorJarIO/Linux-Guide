# Linux Guide
> January 2nd, 2025
---

`cut`: Helps to quickly extract small data sections.

Text File Record Delimiter: A delimiter is one or more characters that create a boundary between different data items within a record. For example, /etc/passwd uses (:) to separate data items within a record. Think of it like the split() method in Python.

The cut command doesn't change any data in a text file. It only copies the data you wish to view and displays it to you.

```bash
cut -d ":" -f 1 /etc/passwd
cut -d ":" -f 1,3 /etc/passwd
cut -d ":" -f 1-3 /etc/passwd

```

`grep`: Uses regular expression to search for text

```bash
grep root /etc/passwd
grep ^root$ /etc/passwd
```

`sort`: Sorts a file's data. Makes no changes to the original file. Only output is sorted

```bash
sort /etc/passwd
sort -n /etc/passwd
```

TO BE CONTINUED
