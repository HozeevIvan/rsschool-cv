# Junior iOS Developer

## Ivan Hozeev

###  Contacts:
  * gmail: __ivanhozeev357@gmail.com__
  * phone: __+ 375 33 345 27 67__
  * LinkedIn: __https://www.linkedin.com/in/ivan-hozeev-98206b192/__

###  About me:
   At 22, I realized that I have a good brain on my shoulders (I am it). This got me to look for a better area to apply my abilities than the job of a cook/waiter, which I got into from the need to start earning for a living early on my own. Since then, I have been consistently moving towards my goal - to become a developer.
What do I want? Become a real expert and be absolutely in demand. To make products of the highest quality, complexity and beauty. Get surrounded by the smartest people in order to become better.

###  About my skills:
#### _Hard_:  
   * **Swift** 
   * **UIKit**
   * Layout & constraints **in code**
   * **Foundation**
   * **Git**
   * **CocoaPods**
 
####  _Soft_:
   * "Master degree" in building good relationships
   * Self management 
   * "Product-oriented thinking"
   * Resolving conflicts in the team
     
###  Latest code examples:

      class NetworkManager {

      static func getWeather(lat: String, lon: String, completionHandler: @escaping (String?, WeatherModelContainer?) -> Void) {
        
        guard let url = URL(string: getUrlString(lat: lat, lon: lon)) else {
            completionHandler("url error", nil)
            return
        }
        
        URLSession.shared.dataTask(with: url) { data, response, error in
            if let data = data {
                do {
                    let decodedResponse = try JSONDecoder().decode(WeatherModelContainer.self, from: data)
                    completionHandler(nil, decodedResponse)
                    print(decodedResponse)
                    return
                } catch {
                    completionHandler(error.localizedDescription, nil)
                    return
                }
            } else {
                completionHandler("unknown error", nil)
                return
            }
            
        }.resume()
      }
      
###  About my experience: 
  * made a simple app with **UITabBarController**,**UITableView**,**Networking** and **Kingfisher pod**
  * made a simple app **UIImagePickerController** and **GestureRecognizers**
  * made a few screens for an app about Fortnite using **GoogleSignIn SDK**,was worked here with a **"keyboard issue"** on **UITextField**
  * made a one screen **weather app** (iOS-native-like) with **Networking** and **UITableView** the link to it below -
   https://bitbucket.org/socialAgent228/mytestweatherapp/src/main/ 

###  About my education:
  * **work with mentor since september 20** (my friend, "middle iOS Dev")
  * **books**, such as: *"Swift (Vasily Usov)"*, *"Programming iOS 14 (Matt Neuburg)"* etc
  * **youTube**: lectures, tutorials
  * **HackerRank** for algorithms
  * **learnAppMaking** website 
  * **internship** in VironIT company (i was quit it, cause it wasnt the real internship)

###  What about *English*?
  * i studied in a gymnasium with a high level of english teaching 
  * in my waiter job it's a common thing to speak with foreign guests
  * related to iOS:
    *  all books that i reading now, they are all in english
    *  a big percent of lectures that i watch - in english too
  * like every other human i have a hobbies, one of them is music and... it's with english speech too :)
