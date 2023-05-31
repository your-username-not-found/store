import random
import string 
def generate_user_agent():

    davik_version = "Davik/2.1.0"

    android_versions = [

        "Android 6.0.0",

        "Android 7.0.0",

        "Android 7.1.0",

        "Android 8.0.0",

        "Android 8.1.0",

        "Android 9.0.0",

        "Android 10.0.0",

        "Android 11.0.0",

        "Android 12.0.0"

    ]

    android_version = random.choice(android_versions)

    g_build = f"{random.choice(string.ascii_uppercase)} Build/{random.randint(1, 9)}"

    fban = "FBAN/FB4A"

    fbav = f"FBAV/{random.randint(100, 999)}.0.0.{random.randint(10000, 99999)}"

    fbbv = f"FBBV/{random.randint(100000000, 999999999)}"

    density = 3.0

    width = 1080

    height = 1920

    fbdm = f"FBDM/{{density={density:.1f},width={width},height={height}}}"

    fblc = "FBLC/en_US"

    fbcr = "FBCR/Rogers"

    fbmf = "FBMF/samsung"

    fbbd = "FBBD/samsung"

    fbdv = "FBDV/SGH-I337M"

    fbsv = "FBSV/5.0.1"

    fbpn = f"FBPN/{random.choice(string.ascii_lowercase)}"

    fbca = "nullFBCA/armeabi-v7a:armeabi;]"

    user_agent = f"{davik_version} (Linux; U; {android_version}; {g_build} [{fban};{fbav};{fbbv};{fbdm};{fblc};{fbcr};{fbmf};{fbbd};{fbpn};{fbdv};{fbsv};{fbca}"

    return user_agent
