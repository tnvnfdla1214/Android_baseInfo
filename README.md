# 안드로이드 기본 지식

## Bundle이란
Bundle은 **여러가지의 타입의 값을 저장하는 Map 클래스**이다.

예를 들면 string 값을 Bundle 클래스에 Mapping(대응, 변환)하는 것이다.

기본타입인 int, double, long, String 부터 FloatArray, StringArrayList, Serializable, Parcelable 까지 구현한다.

Serializable(객체 직렬화)는 객체를 바이트로 저장하는 자바의 인터페이스이고,

Parcelable는 안드로이드에서 만든 것이다.

클래스를 직렬화 하려면, 클래스에  implements Serializable 또는  implements Parcelable을 하여야 한다.

그런데 Android에서는 Activity간에 데이터를 주고 받을 때 Bundle 클래스를 사용하여 데이터를 전송한다.

**bundle의 다른 용도는**
Activity를 생성할 때 아래와 같이 Bundle savedInstanceState 객체를 가지고 와서,

액티비티를 중단할 때 savedInstanceState 메서드를 호출하여 임시적으로 데이터를 저장한다.
즉 전에 저장된 데이터가 있으면, 그 데이터를 가지고 Activity를 다시 생성한다.
