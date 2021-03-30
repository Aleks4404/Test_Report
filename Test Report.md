# Отчёт о тестировании <Credit Card Number Validator>

## Краткое описание

<30.03.2021> - <30.03.2021> Было проведено функциональное тестирование (валидация номеров банковских карт) приложения Credit Card Number Validator.

На тестирование затрачено: <2 часа>

В результате тестирования выявлены следующие дефекты:

* [FAIL при корректном номере карты (American Express) в Credit Card Number Validator](https://github.com/Aleks4404/Test_Report/issues/1)
* [FAIL при корректном номере карты (Diners Club) в коде Credit Card Number Validator](https://github.com/Aleks4404/Test_Report/issues/2)

## Описание процесса тестирования

В процессе тестирования использовались следующие артефакты:
* [Домашнее задание к занятию «1.1. Введение в Java: JDK, JRE, JVM, IntelliJ IDEA»](https://github.com/netology-code/javaqa-homeworks/tree/master/intro)
* [Установка IntelliJ IDEA](https://github.com/netology-code/javaqa-homeworks/blob/master/intro/idea.md)

В качестве тестовых данных использовались валидные и невалидные номера карт, валидные сгенерированы на сайте https://www.freeformatter.com/credit-card-number-generator-validator.html

Валидные номера карт:
* 4929850605056108 - ожидаемый результат - Result is OK.
* 4532657057523629 - ожидаемый результат - Result is OK.
* 55464914677100034 - ожидаемый результат - Result is OK.
* 5351719427810741 - ожидаемый результат - Result is OK.
* 5155809371895414 - ожидаемый результат - Result is OK.

Невалидные номера карт:
* 1111111111111111 - ожидаемый результат - Result is FAIL.
* 1234567890123456 - ожидаемый результат - Result is FAIL.
* 9876543210987654 - ожидаемый результат - Result is FAIL.
* 0000000000000000 - ожидаемый результат - Result is FAIL.
* …………… - ожидаемый результат - Result is FAIL.

Тестирование производилось в следующем окружении:
* Windows 10 Home 64 bit
* версия Java 11.0.10
