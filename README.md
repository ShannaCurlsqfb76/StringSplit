# StringSplit
Func _chargementNews()     $bNews = InetRead("https://127.0.0.1/news.txt",1)     If @error Then MsgBox(64,"ALERT","Impossible de recuperer les News !")     $news = BinaryToString($bNews)     $finalNews = StringSplit($news,"next",1 + 2)     $arraySize = UBound($finalNews)
