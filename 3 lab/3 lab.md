1.
<img width="2378" height="594" alt="image" src="https://github.com/user-attachments/assets/6bfc24cf-9145-4ad6-bab8-51fc3e3a3480" />
2.
<img width="422" height="132" alt="image" src="https://github.com/user-attachments/assets/5cf1abfd-6366-4df7-9396-062e46e838a3" />
3.
<img width="398" height="266" alt="image" src="https://github.com/user-attachments/assets/d32b62d0-dc46-40c0-a8b2-461b7c0adda2" />
4. 
<img width="606" height="330" alt="image" src="https://github.com/user-attachments/assets/b908a0a9-c321-4576-beb9-7955e1a733c6" />
5.
<img width="717" height="324" alt="image" src="https://github.com/user-attachments/assets/306af0d3-ad42-492c-85dd-8d7333aa6c89" />
6.
<img width="668" height="412" alt="image" src="https://github.com/user-attachments/assets/e33f095c-8031-4ec9-a6a6-f00f47d5704b" />
7. 
<img width="338" height="91" alt="image" src="https://github.com/user-attachments/assets/81466899-d62e-4e69-89e1-943ba799f335" />

8. 
#!/bin/bash
if grep -q "^$1:" /etc/passwd; then
    echo "Пользователь $1 найден."
else
    echo "Пользователь $1 не найден."
fi

9.
#!/bin/bash
if grep -q "^$1:" /etc/passwd; then
    echo "Пользователь $1 найден."
else
    echo "Пользователь $1 не найден."
    touch "dont_be_sad_user_$1_will_be_there_soon.txt"
fi

10.
#!/bin/bash
if [ -f "$1" ]; then
    echo "$1 — обычный файл."
elif [ -d "$1" ]; then
    echo "$1 — директория."
elif [ -L "$1" ]; then
    echo "$1 — символическая ссылка."
else
    echo "$1 — не существует или другой тип."
fi

11.
#!/bin/bash
sum=$(( $1 + $2 ))
diff=$(( $1 - $2 ))
prod=$(( $1 * $2 ))
echo "Сумма: $sum"
echo "Разность: $diff"
echo "Произведение: $prod"

12.
#!/bin/bash
for arg in "$@"; do
    echo "$arg"
done

13.
#!/bin/bash
case $1 in
    start) echo "Starting..." ;;
    stop)  echo "Stopping..." ;;
    *)     echo "Используйте: start или stop" ;;
esac

14.
#!/bin/bash
du -sk /home/* 2>/dev/null | sort -nr | awk '{print $2 " — " $1 " КБ"}'

15.
#!/bin/bash
dir="${1:-.}"
find "$dir" -type f -printf '%T@ %p\n' 2>/dev/null | sort -n | head -3 | while read ts path; do
    date=$(date -d "@$ts" "+%Y-%m-%d %H:%M:%S")
    echo "$path — $date"
done

16.
#!/bin/bash
dir="${1:-.}"
size=$(du -sk "$dir" 2>/dev/null | awk '{print $1}')
echo "Общий размер: $size КБ"

17.
#!/bin/bash
hist_file="$HOME/.bash_history"
if [ -f "$hist_file" ]; then
    cat "$hist_file" | awk '{print $1}' | sort | uniq -c | sort -nr | head -5
else
    echo "Файл истории не найден."
fi
