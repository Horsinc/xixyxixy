# Решение определенного интеграла показательной и степенной функции  

## Язык программирования C#
-------------------------------------------------------------------
### Код 
```c#
public string Degree { get; set; }= "";
public string Base { get; set; }= "";

public double OpredIntegral()
{
	if((Degree == "")||(Base == ""))
	{
		return InvalidOperationException("Не введены данные")
	}
	else{
	if((Degree == "x")||(Degree == "X"))
	{
		double basee = Convert.ToDouble(Base);
		return ((Math.Pow(basee, a) / Math.Log(basee)) - ((Math.Pow(basee, b) / Math.Log(basee))));
	}
	else
	{
		double deg = Convert.Todouble(Degree);
		if (deg == -1)
		{
			return InvalidOperationException("Показатель степени = -1")
		}
		else
		{
			return ((Math.Pow(a, deg + 1) / (deg + 1) - ((Math.Pow(b, deg + 1) / (deg + 1)))));
		}
	}
}

public double InvalidOperationException(string v)
{
	throw new NotImplementedException();
}

```
#### Объяснение переменных

***Degree*** - степень (*Глобальная переменная. Тип данных string*)  
**Base** - ~~степень~~ основание (*Глобальная переменная. Тип данных string*)

##### Разбор кода

1. Проверка на "пустоту" вышеперечилсенных переменных
    1. Если да, то вывод ошибки
    1. Если нет - пропуск.
   ```c#
   if((Degree == "")||(Base == ""))
	{
		return InvalidOperationException("Не введены данные")
	}
   ```
1. Пункт 2
    1. Подпункт 2.1. Отступ от трех
    1. Подпункт 2.1. до шести пробелов
1. Пункт 3

   Вложенный текст не менее трех пробелов
1. Пункт 4
