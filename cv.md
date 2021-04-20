#Junior Developer Resume #
##Vitali Leikin##
 **1.Contact Info email:**

> email: <leikin1.19@gmail.com>

 **2.Contact Info Discord**
 > Vitali
 
**3.**
I do my best to get things done.

**4. Skills**

* Objective-C
* Swift
* CocoaPods

**5. Code examples**

```
import UIKit

class ViewController: UIViewController {
    
    @IBOutlet weak var dateTextField: UITextField!
    @IBOutlet weak var monthTextField: UITextField!
    @IBOutlet weak var yearTextField: UITextField!
    @IBOutlet weak var resultLAbel: UILabel! 
    
    @IBAction func myButton(_ sender: UIButton) {        
        guard let day = self.dateTextField.text, let month = self.monthTextField.text, let year = self.yearTextField.text else {return}
        let caledar = Calendar.current
        var dateComponents = DateComponents()
        dateComponents.day = Int(day)
        dateComponents.month = Int(month)
        dateComponents.year = Int(year)
        
        let dateFoemater = DateFormatter()
        dateFoemater.locale = Locale(identifier: "ru_Ru")
        dateFoemater.dateFormat = "EEEE"
        
        guard let date = caledar.date(from: dateComponents) else {return}
   
        let weekday = dateFoemater.string(from: date)
        let capitalizeWeekDay = weekday.capitalized
        self.resultLAbel.text = capitalizeWeekDay
        self.view.endEditing(true)
    }
    
    override func touchesBegan(_ touches: Set<UITouch>, with event: UIEvent?) {
        self.view.endEditing(true)
    } 
}

```
**6. Experience**

To gain experience in programming, I attended various courses and readed  books.

**7. Education**

*I graduated from the Institute of Parliamentarism and Entrepreneurship.
Successfully completed the Siemens Cerberus, Honewell courses on security systems.
I also completed the Institute IBA courses with a degree in System Administrator.*

**8.  Language**

I studied English at school and at university.
Now I attend English courses.