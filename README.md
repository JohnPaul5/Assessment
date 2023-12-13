from binary_search import  binary_search

list = ["Imo state-Owerri", "London-Stoke Newington", "London-Forest Gate", "Southampton-City Centre"]

if input() == ("What locations are available for me to stay?"):
      print(list)
      print("Please enter a desired location if those listed above are satisfactory. If not please input desired location")
      Location = input()
else:
      print("Where would you like to stay?")
      Location = input()

found = binary_search (list, Location)

if found:
      from bed_breakfast_hotel_hostel import binary_search
      list = ["Bed and Breakfast", "Hotel", "Hostel","Villa"]
      input("What type of accomodation would you like to stay in? for your holiday?")
      accomidation = input()
      found = binary_search(list, accomidation)
      if found:
            print("Perfect accomidation in desired location is been sourced")
            from stack import Stacks
            stack = Stack(5)
            stack.push("booked")
      else:
            print("No current location meets your needs.")
else:
      print("Adding location to the database")
      list.append(input())
      from bed_breakfast_hotel_hostel import binary_search
      list = ["Bed and Breakfast", "Hotel", "Hostel", "Villa"]
      input("What type of accomodation would you like to stay in? for your holiday?")
      accomidation = input()
      found = binary_search(list, accomidation)
      if found:
            print("The perfect accomidation in desired location has been found.")
            from stack import Stack
            stack = Stack(5)
            stack.push("booked")
      else:
            print("No current location meets your needs.")
