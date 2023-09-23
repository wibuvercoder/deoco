while True:
    loai_hinh = int(input(" nhập loại hình mà bạn muốn tính diện tích và chu vi : hình chữ nhật(1);tam giác(2);hình vuông(3);hình tròn(4)"))
    if loai_hinh == 1:
        chieu_dai = float(input("nhập chiều dài:"))
        chieu_rong = float(input("nhập chiều rộng:"))
        if chieu_rong>= chieu_dai:
            print("nhập ngu vc")
        else:
            print("chu vi hcn là:",(chieu_dai + chieu_rong)*2,"diện tích hcn là:",chieu_dai*chieu_rong)
        tiep_tuc = str(input("bạn có muốn tiếp tục không : có(a), không(b)"))
        if tiep_tuc.lower() == "a":
            continue
        elif tiep_tuc.lower() == "b":
            print("ok bye")
            break
    elif loai_hinh ==2:
        a = float(input("nhập độ dài cạnh 1 của tam giác:"))
        b = float(input("nhập độ dài cạnh 2 của tam giác:"))
        c = float(input("nhập độ dài cạnh 3 của tam giác:"))
        p = (a+b+c)/2
        if a+b>=c and b+c>=a and a+c>=b and a>0 and b>0 and c>0:
            print("chu vi hình tam giác là:",a+b+c,"diện tích là :",(p*(p-a)*(p-b)*(p-c))**0.5)
        else:
            print(" nhập sai r")
        tiep_tuc = str(input("bạn có muốn tiếp tục không : có(a), không(b)"))
        if tiep_tuc.lower() == "a":
            continue
        elif tiep_tuc.lower() == "b":
            print("ok bye")
            break
    elif loai_hinh == 3:
        canh = float(input())
        print("chu vi hv là:",canh*4,"diện tích là :", canh**2)
        tiep_tuc = str(input("bạn có muốn tiếp tục không : có(a), không(b)"))
        if tiep_tuc.lower() == "a":
            continue
        elif tiep_tuc.lower() == "b":
            print("ok bye")
            break
    elif loai_hinh == 4:
        bk = float(input("nhập bán kính:"))
        print("chu vi hình tròn là:",bk *2*3.14,"diện tích hình tròn là:",(bk**2)*3.14)
        tiep_tuc = str(input("bạn có muốn tiếp tục không : có(a), không(b)"))
        if tiep_tuc.lower() == "a":
            continue
        elif tiep_tuc.lower() == "b":
            print("ok bye")
            break
    else:
        print(" chưa hỗ trợ loại hình này")
        tiep_tuc = str(input("bạn có muốn tiếp tục không : có(a), không(b)"))
        if tiep_tuc.lower() == "a":
            continue
        elif tiep_tuc.lower() == "b":
            print("ok bye")
            break
