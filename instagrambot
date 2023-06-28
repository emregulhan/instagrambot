import instaloader
L = instaloader.Instaloader()



L.login("username","password")  #UPDATE HERE WITH YOUR USERNAME AND PASSWORD.
 

profile = instaloader.Profile.from_username(L.context, "username") #UPDATE HERE AS WELL.

follow_list = []
count = 0
for follower in profile.get_followers():
    follow_list.append(follower.username)


for following in profile.get_followees():
    temp = str(following).split(" ")
    name = temp[1]
    if not name in follow_list:
        print(name)
