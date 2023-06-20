---
layout: post
title: VisionOS 살펴보기
date: 2023-06-20 15:53:00
description: let's get start visionOS
categories: apple visionos vr metaverse
giscus_comments: true
related_posts: true
---

애플이 wwdc2023에서 선보인 Apple Vision Pro의 핵심은 무한한 공간 캔버스이다.
이 광활한 캔버스 위에 간단한 웹사이트 부터 3D 오브젝트까지 모든 것을 보여줄 수 있다. 사용자는 보이는 모든 공간위에서 모든 것을 자유롭게 조작할 수 있으니 사용자 경험이 더욱 유연해진다.

Vision Pro의 운영체제인 VisionOS의 근본을 이루는 3가지 요소는 Windows, Volumes, Spaces 다.

Windows
하나 이상의 windows 를 생성할 수 있다.
SwiftUI의 기존 Windows와 개념은 동일해보인다.
<a href="https://developer.apple.com/documentation/swiftui/windows">swiftui의 Windows</a>

Volumes
VisionOS의 앱은 이제 3D 부피를 가질수 있다.
SwiftUI를 통해 RealityKit이나 Unity와 같이 3D 컨텐츠를 보여줄 수 있다. 깊이를 추가하므로써 앱의 모든 각도에서 컨텐츠를 볼 수 있다.

Spaces
visionOS의 앱은 기본적으로 Shared Space에서 초기화된다.
하나의 Space에서 mac의 데스크탑 앱을 여러개 띄울 수 있다.

## VisionOS을 위한 프레임워크

SwiftUI
visionOS를 위한 최고의 프레임워크이며 기존의 iOS, iPadOS 앱을 visionOS에도 사용할 수 있다.
SwiftUI는 깊이, 제스쳐, 효과, 몰입적 scene과 같이 3D 구현이 쉽다.

RealityKit
애플은 3D 컨텐츠, 애니메이션, 시각적 효과들을 표현하기 위해 3D 렌더링 엔진 RealityKit을 사용하라고 말한다.
RealityKit을 통해 쉽게 구현할 수 있는 부분이 많다.
예를 들어, 물리적 광원 조건과 그림자 생성 등과 같은 것이 있다.

ARKit
우리가 vision pro 시연 영상에서 본 손가락 동작 트래킹에 필요한 기술을 ARKit 프레임워크가 제공한다.
이외에도 Plane Estimation, Scene Reconstruction, Image Anchoring, World Tracking 과 같은 AR에 핵심적인 기술들을 가지고 있다.

Accessibility
visionOS는 접근성을 고려하여 설계되었다.
목소리만으로 동작을 수행하는 것과 같이 제한된 환경에서도 동작가능하다.

## visionOS 개발을 위한 툴

Xcode
Xcode 에는 visionOS SDK가 포함되어 출시된다.
타겟을 visionOS로 지정해야하며, 앱과 상호작용하는 visionOS 시뮬레이터역시 지원된다.

Reality Composer Pro
visionOS 앱을 위한 3D 컨텐츠를 프리뷰할 수 있는 툴이다.
3D 모델, 머터리얼, 음악과 같은 애셋들을 조직화할 수 있다.

Unity
게임 개발에 가장 유명한 툴이다.
passthrough, 동적 시선 추적(Dynamically Foveated Rendering)과 같은 visionOS의 기능들을 그대로 사용할 수 있다.

## visionOS 개발을 위한 준비

visionOS SDK가 공개되기 전까지
<a href="https://developer.apple.com/visionos/prepare/">visionOS 준비하기</a>를 읽어 보자.

wwdc23에서 발표된 visionOS SDK의 <a href="https://developer.apple.com/visionos/learn/">46개의 영상</a>을 공부하자.

---

https://developer.apple.com/visionos/
