# hse_hw2_chip
[Гугл-коллаб](https://colab.research.google.com/drive/109ZMQ3VuESzjCA1PjYzmDa9lysmL6udy?usp=sharing)
# MultiQC

<img width="1104" alt="Снимок экрана 2023-03-01 в 21 31 54" src="https://user-images.githubusercontent.com/99287058/222232191-8fb68090-a89c-49fc-937d-ca4d21a20532.png">
<img width="1104" alt="Снимок экрана 2023-03-01 в 21 32 16" src="https://user-images.githubusercontent.com/99287058/222232367-49acc25b-7cde-41f1-b11e-521bfd5e358d.png">

Подрезать чтения не понадобилось

## Статистика

| образец      | всего выравниваний | выравн. неуникальных| не выравнилось |
| ------------- |------------------| -----| ------- |
| ENCFF000VIP    | 30482497     |  2933620  | 26358118 |
|  ENCFF000VIR   |  26927551| 3523519|22203054 |
| ENCFF000VJK  | 41671673  | 8204532 | 31574789 |

Проанализируйте выдачу bowtie. Почему процент выравниваний получился именно таким?

Процент выравнивания очень низок, потому что мы картируем чтения не на весь геном, а лишь на одну хромосому. Соответственно, риды, не относящиеся к этой хромосоме, не картировались.

## Диаграмы Венна
Сравниваем ENCFF000VIP и ENCODE

<img width="1104" alt="Снимок экрана 2023-03-01 в 21 46 00" src="https://user-images.githubusercontent.com/99287058/222235494-cf0878cc-5288-44d5-ad2e-973f6d710b1f.png">

Сравниваем ENCODE и ENCFF000VIP

<img width="1104" alt="Снимок экрана 2023-03-01 в 21 46 46" src="https://user-images.githubusercontent.com/99287058/222235633-cfb767f9-aa0b-47d5-9181-670a8ca7ab19.png">

Сравниваем ENCFF000VIR и ENCODE

<img width="1104" alt="Снимок экрана 2023-03-01 в 21 47 27" src="https://user-images.githubusercontent.com/99287058/222235779-bec6e9d8-bce2-4509-870d-0c3d0218b5e9.png">

Сравниваем ENCODE и ENCFF000VIR

<img width="1104" alt="Снимок экрана 2023-03-01 в 21 48 00" src="https://user-images.githubusercontent.com/99287058/222235897-78c89be2-a6f3-473e-8c7a-5b7bdfa6967d.png">

2. Проанализируйте полученные результаты и приведите свои рассуждения в README.md. Как можно объяснить различия в количестве пересечений?

Количество пересечений отличается, поскольку в одном случае берутся полученные мной пики, пересекающиеся с пиками ENCODE; а в другом случае отбираются пики ENCODE, совпавшие с пиками, которые получила я.

# Бонус
[Гугл-коллаб](https://colab.research.google.com/drive/1oylmCB2EMnaVDva9Lrr3dejQ2-cmussd?usp=sharing)

|![result](https://user-images.githubusercontent.com/99287058/222255249-75c46c3b-610b-4378-b2e8-597185710a2d.png) | ![result2](https://user-images.githubusercontent.com/99287058/222276324-42686ac9-8380-46af-886c-c0dead12f855.png)|


<img width="562" alt="Снимок экрана 2023-03-01 в 23 19 21" src="https://user-images.githubusercontent.com/99287058/222256319-06a8c35a-69ec-4cfa-bba0-b07ce03d2a86.png">

Полученное распределение совпадает с теоретическим из статьи.


