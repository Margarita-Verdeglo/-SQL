# -SQL
# 1.Создайте функцию, которая принимает кол-во сек и далее переводит их в кол-во дней, часов, минут, секунд.
function secondsToDhms(seconds) {
seconds = Number(seconds);
var d = Math.floor(seconds / (3600*24));
var h = Math.floor(seconds % (3600*24) / 3600);
var m = Math.floor(seconds % 3600 / 60);
var s = Math.floor(seconds % 60);

var dDisplay = d > 0 ? d + (d == 1 ? " day, " : " days, ") : "";
var hDisplay = h > 0 ? h + (h == 1 ? " hour, " : " hours, ") : "";
var mDisplay = m > 0 ? m + (m == 1 ? " minute, " : " minutes, ") : "";
var sDisplay = s > 0 ? s + (s == 1 ? " second" : " seconds") : "";
return dDisplay + hDisplay + mDisplay + sDisplay;
}

# 2.Cоздайте процедуру, которая выведет только числа, делящиеся на 15 или 33 в промежутке от 1 до 1000.

 int n;
    cout << "Enter n: ";
    cin >> n;
    int count = 0;
    for (int i = 1; i <= n; i++)
    {
        if (i % 15 == 0) and (i % 33 == 0)
        {
            count++;
        }
    }
    cout << "Count: " << count << endl;
    system("pause");
    return 0;
