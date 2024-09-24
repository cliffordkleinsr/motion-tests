<script lang="ts">
    import * as Card from "$lib/components/ui/card"
    import AnimatePresenceStack from "$lib/motion/AnimatePresenceStack.svelte";
    import AnimationSequence from "$lib/motion/AnimationSequence.svelte";
    import ColorInterpolation from "$lib/motion/ColorInterpolation.svelte";
    import CyclingThroughStates from "$lib/motion/CyclingThroughStates.svelte";
    import Drag3DTransform from "$lib/motion/Drag3DTransform.svelte";
    import DragConstraints from "$lib/motion/DragConstraints.svelte";
    import DragDirectionLocking from "$lib/motion/DragDirectionLocking.svelte";
    import DragTransform from "$lib/motion/DragTransform.svelte";
    import DurBasedSpring from "$lib/motion/DurBasedSpring.svelte";
    import KeyFramesPostition from "$lib/motion/KeyFramesPostition.svelte";
    import MorphSvg from "$lib/motion/MorphSVG.svelte";
    import Repeat from "$lib/motion/Repeat.svelte";
    import ReverseEffect from "$lib/motion/ReverseEffect.svelte";
    import ScrollProgress from "$lib/motion/ScrollProgress.svelte";
    import Spring from "$lib/motion/Spring.svelte";
    import Tweened from "$lib/motion/Tweened.svelte";
    import WhileDragEffect from "$lib/motion/WhileDragEffect.svelte";
    import WhileHoverEffect from "$lib/motion/WhileHoverEffect.svelte";
    import WhileTapEffect from "$lib/motion/WhileTapEffect.svelte";
</script>
<div class="grid gap-1 m-3 max-w-full">
    <h1 class="text-3xl font-bold mb-2">Functional Tests Motion Start</h1>
    <div class="grid lg:grid-cols-3 gap-2">
        <!-- Start -->
        <Card.Root>
            <Card.Header>
                <Card.Title>
                    Tweened
                </Card.Title>
                <Card.Description>
                    To test click the reload button below
                </Card.Description>
            </Card.Header>
            <Card.Content>
                <Tweened />
            </Card.Content>
            <Card.Footer class="grid gap-1">
                <h1 class="text-2xl font-semibold">Error Summary</h1>
                <p class="text-destructive">Failed Test</p>
            </Card.Footer>
        </Card.Root>
        <!-- End -->
        <!-- Start  -->
        <Card.Root>
            <Card.Header>
                <Card.Title>Spring</Card.Title>
                <Card.Description>
                    To test click the reload button below
                </Card.Description>
            </Card.Header>
            <Card.Content>
                <Spring />
            </Card.Content>
            <Card.Footer>
                <Card.Footer class="grid gap-1">
                    <h1 class="text-2xl font-semibold">Error Summary</h1>
                    <p class="text-destructive">Failed Test</p>
                </Card.Footer>
            </Card.Footer>
        </Card.Root>
        <!-- End -->
        <!-- Start  -->
        <Card.Root>
            <Card.Header>
                <Card.Title>Duration based Spring</Card.Title>
                <Card.Description>
                    To test click the reload button below
                </Card.Description>
            </Card.Header>
            <Card.Content>
                <DurBasedSpring />
            </Card.Content>
            <Card.Footer>
                <Card.Footer class="grid gap-1">
                    <h1 class="text-2xl font-semibold">Error Summary</h1>
                    <p class="text-destructive">Failed Test</p>
                </Card.Footer>
            </Card.Footer>
        </Card.Root>
        <!-- End -->
        <!-- Start  -->
        <Card.Root>
            <Card.Header>
                <Card.Title>Repeat</Card.Title>
                <Card.Description>
                    Just visualize the effect
                </Card.Description>
            </Card.Header>
            <Card.Content>
                <Repeat />
            </Card.Content>
            <Card.Footer>
                <Card.Footer class="grid gap-1">
                    <h1 class="text-2xl font-semibold">Error Summary</h1>
                    <p class="text-destructive">Failed Test</p>
                </Card.Footer>
            </Card.Footer>
        </Card.Root>
        <!-- End -->
        <!-- Start  -->
        <Card.Root>
            <Card.Header>
                <Card.Title>Reverse Effect</Card.Title>
                <Card.Description>
                    Just visualize the effect
                </Card.Description>
            </Card.Header>
            <Card.Content>
                <ReverseEffect />
            </Card.Content>
            <Card.Footer>
                <Card.Footer class="grid gap-1">
                    <p class="text-destructive">Failed Test</p>
                </Card.Footer>
            </Card.Footer>
        </Card.Root>
        <!-- Start  -->
        <Card.Root>
            <Card.Header>
                <Card.Title>While Hover Effect</Card.Title>
                <Card.Description>
                    Hover over the box to visualize the effect
                </Card.Description>
            </Card.Header>
            <Card.Content>
                <WhileHoverEffect />
            </Card.Content>
            <Card.Footer>
                <Card.Footer class="grid gap-1">
                    <h1 class="text-2xl font-semibold">Error Summary</h1>
                    <p class="text-destructive">Failed Test</p>
                </Card.Footer>
            </Card.Footer>
        </Card.Root>
        <!-- End -->
        <!-- Start  -->
        <Card.Root>
            <Card.Header>
                <Card.Title>While Tap Effect</Card.Title>
                <Card.Description>
                    Tap the box to visualize the effect
                </Card.Description>
            </Card.Header>
            <Card.Content>
                <WhileTapEffect />
            </Card.Content>
            <Card.Footer>
                <Card.Footer class="grid gap-1">
                    <h1 class="text-2xl font-semibold">Error Summary</h1>
                    <p class="text-destructive">Failed Test</p>
                </Card.Footer>
            </Card.Footer>
        </Card.Root>
        <!-- End -->
        <!-- Start  -->
        <Card.Root>
            <Card.Header>
                <Card.Title>While Drag Effect</Card.Title>
                <Card.Description>
                    Drag the box to visualize the effect
                </Card.Description>
            </Card.Header>
            <Card.Content>
                <WhileDragEffect />
            </Card.Content>
            <Card.Footer>
                <Card.Footer class="grid gap-1">
                    <h1 class="text-2xl font-semibold">Error Summary</h1>
                    <p class="text-destructive">Failed Test</p>
                </Card.Footer>
            </Card.Footer>
        </Card.Root>
        <!-- End -->
        <!-- Start  -->
        <Card.Root>
            <Card.Header>
                <Card.Title>Cycling through States</Card.Title>
                <Card.Description>
                    Click the box to cycle through different states
                </Card.Description>
            </Card.Header>
            <Card.Content>
                <CyclingThroughStates />
            </Card.Content>
            <Card.Footer>
                <Card.Footer class="grid gap-1">
                    <h1 class="text-2xl font-semibold">Error Summary</h1>
                    <p class="text-destructive">Failed Test</p>
                </Card.Footer>
            </Card.Footer>
        </Card.Root>
        <!-- End -->
        <!-- Start  -->
        <Card.Root>
            <Card.Header>
                <Card.Title>Animation Sequence</Card.Title>
                <Card.Description>
                    Tap the box once to see the animation sequence
                </Card.Description>
            </Card.Header>
            <Card.Content>
                <AnimationSequence />
            </Card.Content>
            <Card.Footer>
                <Card.Footer class="grid gap-1">
                    <h1 class="text-2xl font-semibold">Error Summary</h1>
                    <p class="text-destructive">Failed Test</p>
                </Card.Footer>
            </Card.Footer>
        </Card.Root>
        <!-- End -->
        <!-- Start  -->
        <Card.Root>
            <Card.Header>
                <Card.Title>Drag Constraints</Card.Title>
                <Card.Description>
                    Drag the box visualize the effect
                </Card.Description>
            </Card.Header>
            <Card.Content>
                <DragConstraints />
            </Card.Content>
            <Card.Footer>
                <Card.Footer class="grid gap-1">
                    <h1 class="text-2xl font-semibold">Error Summary</h1>
                    <p class="text-destructive">Failed Test</p>
                </Card.Footer>
            </Card.Footer>
        </Card.Root>
        <!-- End -->
        <!-- Start  -->
        <Card.Root>
            <Card.Header>
                <Card.Title>Drag Direction Locking</Card.Title>
                <Card.Description>
                    Drag the box visualize the effect
                </Card.Description>
            </Card.Header>
            <Card.Content>
                <DragDirectionLocking />
            </Card.Content>
            <Card.Footer>
                <Card.Footer class="grid gap-1">
                    <h1 class="text-2xl font-semibold">Error Summary</h1>
                    <p class="text-destructive">Failed Test</p>
                </Card.Footer>
            </Card.Footer>
        </Card.Root>
        <!-- End -->
        <!-- Start  -->
        <Card.Root>
            <Card.Header>
                <Card.Title>Drag Transform</Card.Title>
                <Card.Description>
                    Drag the box visualize the effect
                </Card.Description>
            </Card.Header>
            <Card.Content>
                <DragTransform />
            </Card.Content>
            <Card.Footer>
                <Card.Footer class="grid gap-1">
                    <h1 class="text-2xl font-semibold">Error Summary</h1>
                    <p class="text-destructive">Failed Test</p>
                </Card.Footer>
            </Card.Footer>
        </Card.Root>
        <!-- End -->
        <!-- Start  -->
        <Card.Root>
            <Card.Header>
                <Card.Title>Drag 3D Transform</Card.Title>
                <Card.Description>
                    Drag the box visualize the effect
                </Card.Description>
            </Card.Header>
            <Card.Content>
                <Drag3DTransform />
            </Card.Content>
            <Card.Footer>
                <Card.Footer class="grid gap-1">
                    <h1 class="text-2xl font-semibold">Error Summary</h1>
                    <p class="text-destructive">Failed Test</p>
                </Card.Footer>
            </Card.Footer>
        </Card.Root>
        <!-- Start -->
        <!-- End -->
        <Card.Root>
            <Card.Header>
                <Card.Title>Color Interpolation</Card.Title>
                <Card.Description>
                    Drag the circle visualize the effect
                </Card.Description>
            </Card.Header>
            <Card.Content>
                <ColorInterpolation />
            </Card.Content>
            <Card.Footer>
                <Card.Footer class="grid gap-1">
                    <h1 class="text-2xl font-semibold">Error Summary</h1>
                    <p class="text-destructive">Failed Test</p>
                </Card.Footer>
            </Card.Footer>
        </Card.Root>
        <!-- End -->
        <!-- Start -->
        <Card.Root>
            <Card.Header>
                <Card.Title>Color Interpolation</Card.Title>
                <Card.Description>
                    Just visualize the effect
                </Card.Description>
            </Card.Header>
            <Card.Content>
                <MorphSvg />
            </Card.Content>
            <Card.Footer>
                <Card.Footer class="grid gap-1">
                    <h1 class="text-2xl font-semibold">Error Summary</h1>
                    <p class="text-destructive">Failed Test</p>
                </Card.Footer>
            </Card.Footer>
        </Card.Root>
        <!-- End -->
        <!-- Start -->
        <Card.Root>
            <Card.Header>
                <Card.Title>Scroll Progress</Card.Title>
                <Card.Description>
                    Drag to visualize the effect
                </Card.Description>
            </Card.Header>
            <Card.Content>
                <ScrollProgress />
            </Card.Content>
            <Card.Footer>
                <Card.Footer class="grid gap-1">
                    <h1 class="text-2xl font-semibold">Error Summary</h1>
                    <p class="text-destructive">Failed Test</p>
                </Card.Footer>
            </Card.Footer>
        </Card.Root>
        <!-- End -->
        <!-- Start -->
        <Card.Root>
            <Card.Header>
                <Card.Title>Keyframes Position</Card.Title>
                <Card.Description>
                    Just visualize the effect
                </Card.Description>
            </Card.Header>
            <Card.Content class="h-[200px] items-center">
                <KeyFramesPostition />
            </Card.Content>
            <Card.Footer>
                <Card.Footer class="grid gap-1">
                    <h1 class="text-2xl font-semibold">Error Summary</h1>
                    <p class="text-destructive">Failed Test</p>
                </Card.Footer>
            </Card.Footer>
        </Card.Root>
        <!-- End -->
        <!-- Start -->
        <Card.Root>
            <Card.Header>
                <Card.Title>Animated Presence Stack</Card.Title>
                <Card.Description>
                    Drag the cards sideways to visualize the effect
                </Card.Description>
            </Card.Header>
            <Card.Content>
                <AnimatePresenceStack />
            </Card.Content>
            <Card.Footer>
                <Card.Footer class="grid gap-1">
                    <h1 class="text-2xl font-semibold">Error Summary</h1>
                    <p class="text-green-500">Passed test</p>
                </Card.Footer>
            </Card.Footer>
        </Card.Root>
        <!-- End -->
    </div>
</div>