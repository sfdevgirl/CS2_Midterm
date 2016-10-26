+CXX = g++
+CXXFLAGS = -Wall -g

all: main.o Utilities.o Customer.o Order.o OrderItem.o MediaItem.o FoodItem.o ElectronicItem.o Date.o 
	$(CXX) $(CXXFLAGS) -o Midterm main.o Utilities.o Customer.o OrderItem.o MediaItem.o FoodItem.o/
		ElectronicItem.o Date.o 

main.o: main.cpp Utilities.hpp Customer.hpp Order.hpp OrderItem.hpp MediaItem.hpp FoodItem.hpp ElectronicItem.hpp Date.hpp 
	$(CXX) $(CXXFLAGS) -c main.cpp 

Utilities.o: Utilities.hpp

Customer.o: Customer.hpp

Order.o: Order.hpp

OrderItem.o: OrderItem.hpp Order.hpp

MediaItem: MediaItem.hpp OrderItem.hpp Order.hpp

FoodItem.o: FoodItem.hpp OrderItem.hpp Order.hpp

ElectronicItem.o: ElectronicItem.hpp OrderItem.hpp Order.hpp

Date.o: Date.hpp

clean:
	rm *.o Midterm
