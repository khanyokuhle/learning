
class AcademicRecord():

    # Obtain student information
    def studentDetails(self):
        self.name = input('Please enter your name: ')
        self.surname = input('Please enter your surname: ')
        self.schoolName = input('Please key in the name of your school: ')

    # Obtain marks from the user
    def getMarks(self):
        try:
            self.english = int(input('Key in your mark for English: \n'))
            while self.english not in range(0,101):
                self.english = int(input('Key in your mark for English: \n'))

            self.mathematics = int(input('Key in your mark for Mathematics: \n'))
            while self.mathematics not in range(0,101):
                self.mathematics= int(input('Key in your mark for Mathematics: \n'))

            self.lifeOrientation = int(input('Key in your mark for Life Orientation: \n'))
            while self.lifeOrientation not in range(0,101):
                self.lifeOrientation= int(input('Key in your mark for Life Orientation: \n'))

            self.history = int(input('Key in your mark for History: \n'))
            while self.history not in range(0,101):
                self.history = int(input('Key in your mark for History: \n'))

            self.computerLiteracy = int(input('Key in your mark for Computer Literacy: \n'))
            while self.computerLiteracy not in range(0,101):
                self.computerLiteracy = int(input('Key in your mark for Computer Literacy: \n'))

            self.art = int(input('Key in your mark for Art: \n'))
            while self.art not in range(0,101):
                self.art = int(input('Key in your mark for Art: \n'))
        except:
            print('Mark entered is not valid, please try again')

    # Calculate yearly average
    def calcAverageYearMark(self):
        average = round((self.english + self.mathematics + self.lifeOrientation + self.history +
                   self.computerLiteracy + self.art)/6, 2)
        if 0.00 < average < 30.00:
            code = '1'
            symbol = 'FF'
            print('Average Year Mark: {} with Symbol {} and code {}'.format(average, symbol, code))
        elif 30.00 <= average < 40.00:
            code = '2'
            symbol = 'F'
            print('Average Year Mark: {} with Symbol {} and code {}'.format(average, symbol, code))
        elif 40.00 <= average < 50.00:
            code = '3'
            symbol = 'E'
            print('Average Year Mark: {} with Symbol {} and code {}'.format(average, symbol, code))
        elif 50.00 <= average < 60.00:
            code = '4'
            symbol = 'D'
            print('Average Year Mark: {} with Symbol {} and code {}'.format(average, symbol, code))
        elif 60.00 <= average < 70.00:
            code = '5'
            symbol = 'C'
            print('Average Year Mark: {} with Symbol {} and code {}'.format(average, symbol, code))
        elif 70.00 <= average < 80.00:
            code = '6'
            symbol = 'B'
            print('Average Year Mark: {} with Symbol {} and code {}'.format(average, symbol, code))
        elif 80.00 <= average <= 100.00:
            code = '7'
            symbol = 'A'
            print('Average Year Mark: {} with Symbol {} and code {}'.format(average, symbol, code))

    # Obtain minimum and maximum marks
    def minMax(self):
        subjects = {'English': self.english, 'Mathematics': self.mathematics, 'Life Orientation': self.lifeOrientation,
                    'History': self.history, 'Computer Literacy': self.computerLiteracy, 'Art': self.art}
        minResult = min(subjects.values())
        maxResult = max(subjects.values())
        print('The highest mark was {}% \nThe lowest mark was {}% \n'.format(maxResult, minResult))

    # Check pass or fail
    def passOrFail(self):
        subjects = {'English': self.english, 'Mathematics': self.mathematics, 'Life Orientation': self.lifeOrientation,
                    'History': self.history, 'Computer Literacy': self.computerLiteracy, 'Art': self.art}
        if subjects['English'] >= 50:
            passCounter = 0
            for subject in subjects.values():
                if subject >= 50:
                    passCounter += 1
            if passCounter >= 4:
                print('Outcome: Passed \n')
            else:
                print('Outcome: Failed \n')
        else:
            print('Outcome: Failed \n')

    # Award distinction
    def awardDistinction(self):
        subjects = {'English': self.english, 'Mathematics': self.mathematics, 'Life Orientation': self.lifeOrientation,
                    'History': self.history, 'Computer Literacy': self.computerLiteracy, 'Art': self.art}
        distinctionList = []
        for k, v in subjects.items():
            if v >= 75:
                distinctionList.append(k)
        print('Subjects paased with Distinction: {}'.format(", ".join(distinctionList)))

    # Obtain symbols and codes for the marks
    def codeSymbol(self):
        subjects = {'English': self.english, 'Mathematics': self.mathematics, 'Life Orientation': self.lifeOrientation,
                    'History': self.history, 'Computer Literacy': self.computerLiteracy, 'Art': self.art}
        print('Subjects'.ljust(30, ' '), 'Mark'.ljust(9, ' '), 'Symbol'.ljust(10, ' '), 'Code'.ljust(7, ' '))
        for k, v in subjects.items():
            if v in range(0,30):
                code = '1'
                symbol = 'FF'
                print(k.ljust(30, ' '), str(v).ljust(3, ' '), '% '.ljust(9, ' '), symbol.ljust(8, ' '), code.ljust(5, ' '))
            elif v in range(30, 40):
                code = '2'
                symbol = 'F'
                print(k.ljust(30, ' '), str(v).ljust(3, ' '), '% '.ljust(9, ' '), symbol.ljust(8, ' '), code.ljust(5, ' '))
            elif v in range(40, 50):
                code = '3'
                symbol = 'E'
                print(k.ljust(30, ' '), str(v).ljust(3, ' '), '% '.ljust(9, ' '), symbol.ljust(8, ' '), code.ljust(5, ' '))
            elif v in range(50, 60):
                code = '4'
                symbol = 'D'
                print(k.ljust(30, ' '), str(v).ljust(3, ' '), '% '.ljust(9, ' '), symbol.ljust(8, ' '), code.ljust(5, ' '))
            elif v in range(60, 70):
                code = '5'
                symbol = 'C'
                print(k.ljust(30, ' '), str(v).ljust(3, ' '), '% '.ljust(9, ' '), symbol.ljust(8, ' '), code.ljust(5, ' '))
            elif v in range(70, 80):
                code = '6'
                symbol = 'B'
                print(k.ljust(30, ' '), str(v).ljust(3, ' '), '% '.ljust(9, ' '), symbol.ljust(8, ' '), code.ljust(5, ' '))
            elif v in range(80, 101):
                code = '7'
                symbol = 'A'
                print(k.ljust(30, ' '), str(v).ljust(3, ' '), '% '.ljust(9, ' '), symbol.ljust(8, ' '), code.ljust(5, ' '))

    # Display the report
    def display(self):
        self.studentDetails()
        self.getMarks()
        print('\n**********************************************************')
        print('STUDENT ACADEMIC RECORD'.rjust(30, ' '))
        print('This program inputs the learner marks of matric \nlevel subjects and prints the student final report.')
        print('**********************************************************\n')
        print('Name: {} {}    School: {}\n'.format(self.name, self.surname, self.schoolName))
        self.codeSymbol()
        self.calcAverageYearMark()
        self.passOrFail()
        self.minMax()

x = AcademicRecord()
x.display()
