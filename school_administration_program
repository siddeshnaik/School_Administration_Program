import csv

def csv_file_writing(info_list):
    with open("student_info_new.csv" , "a" ,newline='') as csv_file:
        writer_of_file = csv.writer(csv_file)
        
        if(csv_file.tell() == 0):
            writer_of_file.writerow(info_list)
        
        else:
            writer_of_file.writerow(info_list)    
    

if __name__ == '__main__':
    category_condition = True
    index_of_category = 0
    category_list=["bro"]
    category_list.clear()
    while(category_condition):
            category_list.append(input("What do you want the column to be about "))

            print("Entered column name is ",category_list[index_of_category])            
            
            correction_check=input("Enter Y/N if data is correct/incorrect")
            
            if(correction_check.upper() == "Y"):

                category_condition_check=input("Enter Y/N if you want to enter a new column/no new column")
                
                if (category_condition_check.upper() == "Y"):
                    category_condition = True
                    index_of_category=index_of_category + 1                   

                elif(category_condition_check.upper() == "N"):
                    category_condition = False 

                
            
            elif(correction_check.upper() == "N"):
                print("Enter the column again")
                category_list.pop()
        
            else:
                print("Since a valid entry wasn't entered it automatically added a new data set")
            
        
    print("The entered columns are ",category_list)
    
    csv_file_writing(category_list)
    i=0
    for ele in category_list:
        i=i+1
        
    print("Number of columns are ",i)

    student_info_list=["text"]
    student_info_list.clear()
    condition=True
    while(condition):
            for x in range(0,i):
                student_info_list.append(input("Enter the {} of the student ".format(category_list[x])))
            
            #print("Entered Data is",student_info_list)
            for y in range(0,i):
                print(category_list[y]," : ",student_info_list[y])
                
                
            correction_check=input("Enter Y/N if data is correct/incorrect ")
            
            if (correction_check.upper() == "Y"):
                csv_file_writing(student_info_list)
                category_condition_check=input("Enter Y/N if you want to enter information of a new student/or not ")
                
                if (category_condition_check.upper() == "Y"):
                    condition = True
                
                elif(category_condition_check.upper() == "N"):
                    condition = False
                    
                else:
                    print("Since a valid entry wasn't entered it automatically added a new data set ")
                
            elif(correction_check.upper()== "N"):
                print("Enter the Values again")
                
            else:
                print("Since a valid entry wasn't entered data is discarded please re-enter the values ")
                
            student_info_list.clear()
    
