Senior group
class Child:
    def __init__(self, name, age):
        self.name = name
        self.age = age

    def __str__(self):
        return f"Имя: {self.name}, Возраст: {self.age}"

class Group:
    def __init__(self, group_name):
        self.group_name = group_name
        self.children = []

    def add_child(self, child):
        self.children.append(child)

    def display_group_info(self):
        print(f"Группа: {self.group_name}")
        for child in self.children:
            print(child)

# Создание объектов детей
child1 = Child("Маша", 4)
child2 = Child("Ваня", 5)
child3 = Child("Катя", 3)

# Создание объекта группы
group = Group("Старшая группа")

# Добавление детей в группу
group.add_child(child1)
group.add_child(child2)
group.add_child(child3)

# Отображение информации о группе
group.display_group_info()

