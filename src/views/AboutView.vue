<template>
    <div class="about">
        <h1>This is an about page</h1>
        <Button type="primary">Primary</Button>
        <hr />
        <div style="height: 10rem">
            <Carousel v-model="value" loop>
                <CarouselItem v-for="item in 3" :key="item">
                    <div class="demo-carousel">
                        <img
                            alt="Vue logo"
                            :src="require(`@/assets/Images/avatar/${item}.jpg`)"
                        />
                    </div>
                </CarouselItem>
                <!-- <CarouselItem>
                    <div class="demo-carousel">2</div>
                </CarouselItem>
                <CarouselItem>
                    <div class="demo-carousel">3</div>
                </CarouselItem>
                <CarouselItem>
                    <div class="demo-carousel">4</div>
                </CarouselItem> -->
            </Carousel>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            value: 0,
        };
    },
};
</script>
