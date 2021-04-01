# Отчёт о тестировании <Credit Card Number Validator>

## Краткое описание

<30.03.2021> - <30.03.2021> Было проведено функциональное тестирование (валидация номеров банковских карт) приложения Credit Card Number Validator.

На тестирование затрачено: <2 часа>

В результате тестирования выявлены следующие дефекты:

* [Сообщение Result is FAIL при проверке кода программы корректным номером карты](https://github.com/Aleks4404/Test_Report/issues/1)
* [Сообщение Result is FAIL при проверке кода программы корректным номером карты](https://github.com/Aleks4404/Test_Report/issues/2)

## Описание процесса тестирования

В процессе тестирования использовались следующие артефакты:
* [Домашнее задание к занятию «1.1. Введение в Java: JDK, JRE, JVM, IntelliJ IDEA»](https://github.com/netology-code/javaqa-homeworks/tree/master/intro)
* [Установка IntelliJ IDEA](https://github.com/netology-code/javaqa-homeworks/blob/master/intro/idea.md)

В качестве тестовых данных использовались валидные и невалидные номера карт, валидные сгенерированы на сайте https://www.freeformatter.com/credit-card-number-generator-validator.html

Валидные номера карт:
VISA:
* 4716159148446538 - ожидаемый результат - Result is OK
* 4929688265750762 - ожидаемый результат - Result is OK
* 4539917862079137368 - ожидаемый результат - Result is OK

MasterCard:
* 5230479895009410 - ожидаемый результат - Result is OK
* 5158917014078921 - ожидаемый результат - Result is OK
* 5586377820992058 - ожидаемый результат - Result is OK

American Express (AMEX):
* 344526600602089 - ожидаемый результат - Result is OK
* 377813276481380 - ожидаемый результат - Result is OK
* 373825299665876 - ожидаемый результат - Result is OK

Visa Electron:
* 4844634278855455 - ожидаемый результат - Result is OK
* 4175001608229687 - ожидаемый результат - Result is OK
* 4913560635377238 - ожидаемый результат - Result is OK

Невалидные номера карт:
* 1111111111111111 - ожидаемый результат - Result is FAIL.
* 1234567890123456 - ожидаемый результат - Result is FAIL.
* 9876543210987654 - ожидаемый результат - Result is FAIL.
* 0000000000000000 - ожидаемый результат - Result is FAIL.
* …………… - ожидаемый результат - Result is FAIL.

Тестирование производилось в следующем окружении:
* Windows 10 Home 64 bit
* версия Java 11.0.10