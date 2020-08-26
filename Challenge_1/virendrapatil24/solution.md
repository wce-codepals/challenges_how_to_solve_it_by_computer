def challenge():

	print("Welcome to Challenge 1 Solution...!!!")

	get_solution()


def get_solution():

	colors = int(input("Enter number of different colors:"))

	if colors == 1:

		print("You already have your solution.") #It can be a case where user wants to check the answer.

	elif colors == 2:

		get_numcolor2()

	elif colors == 3:

		get_numcolor3()

	else:

		print("Wrong Input!")

		get_solution()


def get_numcolor2():

	blocks = int(input("Enter total number of blocks:"))

	if blocks == 1:

		print("You already have your solution.") #2 colors and 1 block not possible as user has got solution already.

	elif blocks == 2:

		print("Select color from any block and tap to another block and you will get your solution.")

	elif blocks > 2:

		print("Find the block (say B1) which is between 2 blocks having same color (say C1), then select C1 and tap B1.")

		get_solution()


def get_numcolor3():

	blocks = int(input("Enter total number of blocks:"))

	if blocks == 1:

		print("You already have your solution.") #2 colors and 1 block not possible as user has got solution already.

	elif blocks == 2:

		print("Wrong Input!") #3 colors and 2 blocks are not possible.

		get_solution()

	elif blocks == 3:

		print("Select color from any block (say B1) and tap on any block (say B2).")

		get_solution()

	elif blocks > 3:

		print("Find the block (say B1) which is between 2 blocks having same color (say C1), then select C1 and tap B1.")

		get_solution()
