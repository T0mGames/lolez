def check_tri_type_by_angle(sides: list):
    a, b, c = list(map(int, sides))
    if (a+b+c) > 180: 
        return "Not a triangle"
    

    dupeCheck = [int(x) for n, x in enumerate(sides) if x in sides[:n]]
    nonDupes = [int(x) for n, x in enumerate(sides) if x not in sides[:n]]
    if len(dupeCheck) == 2:
        return "Equalateral"
    elif len(dupeCheck) == 1:
        return "Iscocoles"
    else:
        return "Scalene"
    
    return "Not a triangle"

def check_tri_type_by_sides(sides: list):
    a, b, c = list(map(int, sides))
    assert(a+b>=c and b+c>=a and c+a>=b)
    if a==b and b==c:
        return "Equalateral"
    elif a==b or b==c or a==c:
        return "Iscocoles"
    else:
        return "Scalene"


angles = ["50", "60", "70"]
triType = check_tri_type_by_angle(angles)
print(f"Triangle type is: {triType}")

triType2 = check_tri_type_by_sides([100, "50", 50])
print(f"Triangle type is: {triType2}")


