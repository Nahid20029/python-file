class Appliance:
    def __init__(self, brand, power):
        self.brand = brand
        self.power = power
    def info(self):
        print(f"The appliance from {self.brand} uses {self.power} watts of power.")
class Refrigerator(Appliance):
    def __init__(self, brand, power, capacity):
        super() .__init__(brand, power)
        self.capacity = capacity
    def info(self):
        print(f"The refrigerator from {self.brand} has a capacity of {self.capacity} liters and uses {self.power} watts of power.")
class WashingMachine(Appliance):
    def __init__(self, brand, power, load_capacity):
        super().__init__(brand,power)
        self.load_capacity = load_capacity
    def info(self):
        print(f"The washing machine from {self.brand} has a load capacity of {self.load_capacity} kg and uses {self.power} watts of power.")
fridge = Refrigerator("samsung", 150, 350)
washing_machine = WashingMachine("LG", 500, 7)

fridge.info()
washing_machine.inf
